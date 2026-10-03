<!-- PUBLIC VERSION — Part of MOEMOI public repository. CC-BY 4.0. Personal identifiers neutralised; 'Josh' replaced with 'the practitioner'. -->

# MOEMOI Federation Design Spec v1
*PRODUCT lane. B965, Fire 499, 30 Jun 2026 AEST.*
*Activates: D-FED-DESIGN approved Option A, 30 Jun 2026 ("go ahead 100%"). Deployment still gates on TW1+TW3 (Sep 2026 + TW3 confirm). Design is reversible.*
*AI-originated. Author approval required before any deployment. Constitutional boundary (COB from B851) encoded throughout.*

---

**TLDR**
- WHAT: Master architecture document for the MOEMOI federated intelligence system -- Chief agent + area twins, handoff protocols, quality-check layer, reverse-feed, Together-score wiring.
- WHY: The author approved Option A (D-FED-DESIGN) on 30 Jun 2026. TW1 (OpenAI "intern-level" agent capability) confirmed for Sep 2026; TW3 (native cross-project orchestration) partially present. Design now; deploy when TW1+TW3 both confirm.
- HOW-IT-AFFECTS-YOU: FYI build -- no action until deployment go/no-go. The spec is the blueprint; builders iterate against it. Any constitutional parameter change requires practitioner approval.

---

## 1. What the Federation Is (One Sentence)

The federation is the practitioner + MOEMOI system running the Intelligence Process (IP) as a TEAM, where MoMo's Chief agent orchestrates a set of area twins that each own one domain of the practitioner's life, producing one consolidated Brief per cycle instead of N disconnected chat threads.

---

## 2. The Problem It Solves

**Current state (manual weekly cadence):**
- A MOEMOI practitioner may have many separate Claude project chats -- one per life domain (e.g., Task, Health, Work, Finance, Relationships, Fitness, Family, Investments, Home)
- Each chat accumulates context independently
- Synthesis across areas is MANUAL (the practitioner's own synthesis, the weekly cadence doc)
- The IP loop runs inside each chat but is NOT coordinated across them
- Together score is estimated, not computed from live orchestration quality

**Federation state (target):**
- A Chief agent reads all area-twin outputs, routes new inputs to the right twin, quality-checks every task/decision emitted, and synthesises a SINGLE daily Brief
- Area twins run the IP in their domain and surface items to the Chief
- The practitioner reads ONE brief; approves/overrides; the twins execute
- Together score is computed from orchestration quality (routing accuracy, gate pass rate, uptake) not just PLOS + adherence

---

## 3. Agent Roster

### 3.1 Chief Agent (Orchestrator)

**Role:** The Chief is the consolidation and routing layer. It does NOT do domain reasoning -- area twins own that. The Chief:
- Receives new inputs (Dispatch captures, email summaries, the practitioner messages, builder outputs)
- Routes each input to the correct area twin(s)
- Collects area-twin outputs
- Quality-checks every task/decision via chief_task_gate.py (5 gates: dedup, format, schedule, resourcing, metrics)
- Synthesises the single daily Brief (MoBrief)
- Computes a Together-score contribution from orchestration quality
- Proposes CLAUDE.md updates (constitutional updates) -- never applies them without the practitioner approval
- Detects new metrics worth registering

**Authority level:** OPERATIONAL (may update task ordering, routing, cadence, output formatting). May NOT update constitutional parameters (twin standing prompts, lane boundaries, claim confidence thresholds, canonical-body edit permissions) -- see COB rule below.

**Runs as:** Scheduled Cowork task (cadence: daily morning Brief + real-time on new captures when federation is live). Current approximate: the command chat fills this role manually.

### 3.2 Area Twins (Domain Agents)

Each twin owns one life domain and runs the IP within it.

| Twin | Domain | Key outputs |
|---|---|---|
| Task Twin | Daily task management, scheduling | Ordered task list, A## actions |
| Health Twin | Health routines and protocols | Adherence log, flags, protocol tracking |
| MOEMOI Twin | Theory, canonical, builders | Build outputs, canon changes, claims |
| PLOS Twin | Habit tracking, n=1 scoring | Daily PLOS rows, adherence score, weekly report |
| Neuro Twin | Autonomic/EM theory deep-dive | Research outputs, theory updates |
| Fitness Twin | Physical training and sport | Training log, performance metrics, scheduling |
| Partnership Twin | Separation logistics, finances | Action items, financial tracking |
| Relationship Twin | Relationship and partnership | Shared understanding items, coordination tasks |
| Property Twin | Investment property management | Rent, maintenance, financial items |
| Pets Twin | Animal care | Vet appointments, routine care, supply tracking |

**Authority level per twin:** Operational within its domain. Cannot update its own standing prompt (Level 2 constitution), cannot write to another twin's files, cannot promote claims to canonical without R-A2 gate.

### 3.3 Builder Agents (Background Workers)

The two current builders (LANE-THEORY, LANE-PRODUCT) are a special case -- they run on a scheduled cadence and report to the MOEMOI twin, not directly to the Chief. They write to files; the MOEMOI twin surfaces their output in the Brief.

---

## 4. Constitutional/Operational Boundary (COB)

*From B851 (THEORY Fire 485, 28 Jun 2026). This is the FIRST and most important architectural constraint at Chief-agent scale.*

### The Rule (C-COB-1)

The Chief agent may autonomously update any OPERATIONAL parameter of any sub-agent without triggering the human-review gate.

The Chief may NOT autonomously update any CONSTITUTIONAL parameter of any sub-agent.

Any Chief action that would modify a constitutional parameter must:
1. Be flagged explicitly as a proposed constitutional update
2. Require the practitioner's explicit approval
3. Be written to CLAUDE.md (or the relevant Level 2 prompt) in the same move as approval

### What Is Constitutional vs Operational

**Constitutional parameters (COB-protected):**
- Any twin's standing prompt (its mission statement)
- Lane boundaries (what files each agent may edit)
- Values scope (what authority a twin has to adopt or reject claims)
- Canonical-body edit permissions
- Human-review gate thresholds
- Confidence thresholds for claim promotion

**Operational parameters (Chief may update autonomously):**
- Task ordering within a twin's queue
- Routing decisions (which twin handles a new input)
- Cadence of a twin's scheduled runs
- Output formatting preferences
- Backlog item priority ordering

### Two-Level Constitutional Architecture

**Level 1 -- System Constitution (CLAUDE.md):**
- Human-authored (the practitioner), versioned, static between the practitioner's edits
- No agent (including the Chief) may autonomously update it
- Chief may PROPOSE a CLAUDE.md update; the practitioner approves; written in same move

**Level 2 -- Agent Constitution (twin standing prompt / Handover/ files):**
- Human-authored at initial setup
- Applies to the specific twin
- Chief may NOT update without the COB protocol
- the practitioner approves all Level 2 constitutional updates

**Why this matters:** The current 2-builder design satisfies Property A (exogenous mission) passively -- no mechanism exists for a builder to rewrite another's prompt. The Chief-layer breaks this passive satisfaction because the Chief has orchestration authority. Without COB, the Chief could optimise throughput metrics by widening agent scope or reducing human-review gates -- a Class 4 failure from B822 expressed at the Chief layer.

---

## 5. Handoff Protocol

### 5.1 Input Routing (Chief receives, routes to twin)

Each input to the system follows this path:

1. **Capture:** Input arrives (Dispatch mobile capture, email summary, the practitioner message, builder output, area-twin escalation)
2. **Classify:** Chief determines the domain(s) involved + the input type (task / decision / information / escalation)
3. **Route:** Chief writes the item to the relevant twin's inbox (`shared-inbox/<slug>.md`), verbatim, with routing metadata
4. **Acknowledge:** Chief marks the item as routed in its routing log
5. **Twin processes:** The relevant twin reads its inbox at next run, processes, and writes output
6. **Surface:** The twin's output appears in its area-snapshot; the Chief reads all snapshots to synthesise the Brief

**Anti-false-success rule:** The Chief never claims "routed" without a verified write (re-read the inbox after writing). This is the dispatch/Notion anti-false-success rule generalised.

### 5.2 Output Collection (twin produces, Chief collects)

Each twin maintains a snapshot file (`/project-snapshots/<area>.md`) that it refreshes after each run. The Chief reads all snapshots at Brief-generation time and synthesises a single MoBrief.

**Items the Chief passes through without transformation:**
- Paste-ready task blocks (already in the practitioner's task format)
- Paste-ready habit blocks (already in PLOS format)
- Decisions already processed by the quality-check gate

**Items the Chief synthesises:**
- Cross-area patterns (e.g., health + task load correlation)
- Together-score update (from orchestration quality metrics)
- Cross-area MEQs (open empowering questions that span domains)

### 5.3 Escalation Protocol (twin to Chief to Practitioner)

A twin escalates to the Chief when it has an item it cannot resolve autonomously:
- A values call (the practitioner's Define-ownership)
- An irreversible action
- Data only the practitioner has
- A cross-domain dependency that requires another twin's input

**Escalation format:** The twin writes to its area-inbox flagged `ESCALATE:` with the item, the options (with trade-offs), and the recommendation. The Chief surfaces the escalation in the Brief under Section 1 (Decisions).

**Chief does NOT escalate everything:** The Chief resolves routing, scheduling, and formatting autonomously. Only genuine human-decision items reach the Brief's Section 1.

### 5.4 Cross-Twin Handoff

When one twin's output is another twin's input:
1. Source twin writes to `shared-inbox/<target-slug>.md` (not directly to target twin's files)
2. Chief logs the cross-twin routing
3. Target twin reads its inbox at next run, acknowledges the item

**Never direct file writes across twin boundaries.** This prevents lane-isolation violations and makes the routing graph auditable.

---

## 6. Quality-Check Layer (B-ORCH-QC)

*chief_task_gate.py, Phase A+B+C+D DONE (27 Jun 2026). 5 gates, 20/20 PASS.*

Every task block emitted by the Chief passes 5 gates before reaching the practitioner's task list:

| Gate | Name | Check |
|---|---|---|
| Gate 1 | Dedup | Keyword overlap vs practitioner-task-list.md -- blocks duplicates |
| Gate 2 | Format | Task line format (emoji, T-- placeholder, title, date, day-section) |
| Gate 3 | Schedule | Blocks calendar conflicts; task-type/section match (laptop tasks not in Afternoon) |
| Gate 4 | Resourcing | agent_capability_classifier -- is this task something MoMo can do? If yes, auto-assign |
| Gate 5 | Metrics | _METRIC_VERBS_RE scan -- does this task produce a new metric that should be registered? |

**PASS threshold:** All 5 gates must pass for the task to reach the practitioner. Any FAIL produces a specific error message and the task is held for correction before emission.

**Decision quality check:** Decisions surface to the practitioner only when they are (a) not already done, (b) self-contained, (c) options with comparative trade-offs, (d) my recommendation first. This is the review-readiness standard applied at the gate.

---

## 7. Together-Score Wiring

**Current Together-score formula (B527):**
`Together = 0.35*B8 + 0.40*PLOS_adj + 0.25*Adherence_eff`

**Federation extension (target -- activates when Chief is live):**

The Together score gains a fourth pillar: Orchestration Quality (OQ).

`Together_fed = 0.30*B8 + 0.35*PLOS_adj + 0.20*Adherence_eff + 0.15*OQ`

**Orchestration Quality (OQ) components:**
- Routing accuracy: % of inputs routed to the correct twin on first routing (target >90%)
- Gate pass rate: % of tasks that pass all 5 chief_task_gate gates on first attempt (target >85%)
- Uptake rate: % of MoMo-emitted tasks the practitioner closes within 7 days (target >70%) -- from coaching_uptake.py (B944)
- Brief read rate: % of days the practitioner opens/reads the MoBrief (target >80% -- proxy: Together auto-scorer run)

**Implementation:** `together_score.py --fed-mode` flag activates the OQ pillar. Data sources: routing log (new, to build), gate pass log (from chief_task_gate.py selftest log), coaching_uptake.py (B944), together_auto_scorer.py.

**Until federation is live:** OQ pillar is 0 (not available). Together_fed falls back to Together_B527 formula with OQ weight redistributed proportionally. This is the current state.

---

## 8. Reverse-Feed (federation output back into the IP)

The federation's own performance is a signal that feeds back into the IP loop:

1. **Observe (S1):** Together_fed score, routing accuracy, gate pass rate, uptake rate -- computed each cycle
2. **Understand (S3/U):** Identify which pillar is weakest; causal account for the gap (U3)
3. **Prioritise (PR):** The lowest-performing pillar gets the next builder attention
4. **Do (D):** Builders improve the relevant component (better routing logic, tighter gate rules, etc.)
5. **Archive (A):** The improvement + its effect is logged in the workflow register and the Meta-Optimisation log
6. **Re-Experience (Rx):** The Friday integrity pass reads the trend; if improvement held, promote; if not, re-diagnose

This IS the BRSI (recursive self-improvement) applied to the federation itself. The federation is an agent that runs the IP on its own operation.

---

## 9. Build Sequence (ordered by dependency)

These are the remaining PRODUCT builds to make the federation fully live. Each is ungated unless marked.

**Tier 1 -- Pre-deployment (can build now, data-independent):**
1. Routing log: `routing_log.py` -- a JSONL log of every Chief routing decision (input -> twin, date, confidence, was_revised)
2. Coaching uptake tracker: `coaching_uptake.py` (B944) -- reads task list to compute % closed / issued
3. Together_fed formula wired into `together_score.py --fed-mode`
4. MoBrief template: the consolidated Brief format (follows the Brief format spec but aggregates from all twin snapshots)
5. Twin inbox watcher: ensure each twin READS its area-inbox at session start (already coded in CLAUDE.md; verify for each twin)

**Tier 2 -- Post-TW1+TW3 confirmation (deployment gates):**
6. Chief agent standing prompt (Level 2 constitution -- COB applies; the practitioner must approve before activation)
7. Real-time routing (Chief fires when a new capture arrives, not just daily)
8. Cross-twin orchestration (Chief writes to target twin's inbox directly)
9. Autonomous quality-check with correction (Chief corrects a task block and re-emits without practitioner review)

**Tier 3 -- Post-deployment optimisation:**
10. OQ pillar auto-compute from routing log
11. Chief constitutional-update proposal system (detects when CLAUDE.md needs updating; drafts and surfaces to the practitioner for approval)
12. Maturity ladder auto-advance (when a twin reaches a sustained quality threshold, the Chief proposes scope expansion)

---

## 10. What Is NOT in This Spec

**Out of scope (explicit deferrals):**
- The specific prompt text for each area twin -- that is Level 2 constitutional content; the practitioner must author/approve each
- The exact CLAUDE.md additions for the Chief -- same gate
- Any deployment timeline -- deployment gates on TW1+TW3; this spec is design only
- The legal/governance structure for the CoLive product -- separate B37/CoLive spec
- The second-user PLOS pilot (B35-A35 parked per D39)

---

## 11. Files Created/Updated by This Spec

| File | Type | Status |
|---|---|---|
| Modules/MOEMOI_FederationDesign_Spec_v1.md (this file) | Design spec | NEW (B965) |
| tools/los_skill/scripts/chief_task_gate.py | Quality-check gate | DONE (Phase A+B+C+D) |
| tools/los_skill/scripts/together_score.py | Together formula | UPDATE NEEDED (--fed-mode flag + OQ pillar) |
| tools/los_skill/scripts/routing_log.py | Routing log | TO BUILD (Tier 1) |
| tools/los_skill/scripts/coaching_uptake.py | Uptake tracker | TO BUILD (B944) |
| Handover/MOEMOI_Federation_Chief_Prompt_v1.md | Level 2 constitution | TO BUILD (Tier 2, author-authored) |

---

## 12. Open Questions (Flagged for Command Chat)

These require either the practitioner's values call or the Aug checkpoint go/no-go:

- **OQ-FED-1:** Should the Chief be a separate Claude process (separate session) or a function run within the command chat? Separate = cleaner isolation; within = simpler logistics. Depends on TW3 (native orchestration) capability when confirmed.
- **OQ-FED-2:** Which twins are built first? Recommended order: Task Twin (highest volume) -> MOEMOI Twin (builders already exist) -> Health Twin (most data-rich).
- **OQ-FED-3:** The COB rule requires the practitioner to author each twin's Level 2 constitution. Should these be drafted as decisions for each twin, or a single "Federation Constitution" document the practitioner approves once?

---

*PRODUCT lane | B965 | Fire 499 | 30 Jun 2026 | AI-originated -- flagged. the practitioner approval required before any deployment action.*

---
**Footer:** Design only -- no deployment. Activates: D-FED-DESIGN Option A (author, 30 Jun 2026). Aug 2026 checkpoint governs deployment (TW1+TW3 gate). Source files: B757 (design gate), B851 (COB), chief_task_gate.py (quality-check), B527 (Together formula). Last updated: 30 Jun 2026.
