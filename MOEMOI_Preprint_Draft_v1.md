# MOEMOI: A Universal Intelligence Process Framework for Human Optimisation


---

## Abstract

We present the MOEMOI (Most Optimal and Ever-More-Optimal Intelligence) framework, which argues that all intelligent systems (biological, social, and artificial) execute a single recursive process (the Intelligence Process, or IP) when they improve. Unlike existing memory-governance frameworks, which govern how AI systems retain and retrieve information, MOEMOI introduces the first ends-governance layer over the retention function: what the system retains is authorised by the practitioner's own goal-definition quality, not only the agent's consolidation algorithm (C133, ADOPTED, confidence 0.86). The framework is accompanied by a confidence-graded claims register (165 claims, 82 adopted at high confidence) that makes its epistemic commitments explicit, sortable, and falsifiable. Confidence scores in the register are not Bayesian probabilities but structured epistemic grades (HYPOTHESIS, CANDIDATE, ADOPTED, ARCHIVED, HELD), with criteria for each tier described in Section 5. We derive the framework from three independent routes: (1) the logical conditions for any system to improve at improving, (2) the intersection of thermodynamic self-organisation and Bayesian active inference, and (3) the 4E cognition tradition (Varela, Thompson, and Rosch 1991; O'Regan and Noë 2001), all of which converge on the same six-step architecture comprising six substeps: Experience, Understand, Prioritise, Define, Prepare, and Do/Learn (abbreviated EUPDDL). We show that twenty-one existing frameworks, including OODA (Observe, Orient, Decide, Act), the scientific method, PDCA (Plan, Do, Check, Act) cycle, and active inference, are specialist frameworks that each provide genuine depth at specific substeps of the IP; MOEMOI provides the unifying architecture that contextualises their contributions. We propose a four-level obstacle taxonomy (grounded in Freud, Sartre, Wollstonecraft, and functional medicine / disability studies) that classifies recurring implementation failures into personal-structural, phenomenological, sociological-structural, and biological-somatic types, with distinct intervention prescriptions for each. We describe preliminary practitioner implementation as a Life Operating System (LOS), outline the conditions under which the framework would be disconfirmed, and discuss the multi-agent extension. The framework is released under Creative Commons Attribution 4.0 (CC-BY 4.0).


**Keywords:** intelligence theory, optimisation, life operating system, OODA, active inference, self-directed improvement, recursive self-improvement, personal operating systems

---

*First-time readers: a glossary defining EUPDDL, IP, LOS, void taxonomy, claims register tiers, and all acronyms is available in MOEMOI_Glossary_v1.md (this repository) or as Appendix C in the full canonical.*

## 1. Introduction

The most consequential skill there is, how to live and make decisions well, is the least systematised. Humanity has formalised mathematics, medicine, software engineering, and hundreds of other domains into teachable, improvable bodies of knowledge with standards, institutions, and accumulated method. For the question of how to be a person and direct one's own life well, the field offers thousands of books and traditions, each claiming authority, none of which make their reasoning structure explicit enough to be tested, compared, or improved collectively.

This paper presents MOEMOI, a framework that attempts to provide what is missing: a single, clear, teachable, and falsifiable account of the process by which any intelligent system, a person, a team, an artificial agent, or a civilisation, moves from its current state toward a more optimal one, recursively and without a fixed ceiling.

The central claim is straightforward: when any intelligent system improves, it does so by running one process. That process has a fixed logical structure, derivable from first principles. Running it more completely, more accurately, and more frequently is what improvement means. The framework does not prescribe what to optimise for, that remains the practitioner's domain, but it does describe the structure of optimisation itself.

MOEMOI is not primarily a self-help system, though it has practitioner applications. It is a claim about the structure of intelligence, advanced at the level of a theoretical framework and evaluated against alternative accounts of intelligent behaviour, learning, and decision-making.

We present the MOEMOI framework, which argues that all intelligent systems (biological, social, and artificial) execute a single recursive process (the Intelligence Process, or IP) when they improve. Unlike existing memory-governance frameworks, which govern how AI systems retain and retrieve information, MOEMOI introduces the first ends-governance layer over the retention function: what the system retains is authorised by the practitioner's own goal-definition quality, not only the agent's consolidation algorithm (C133, confidence 0.86, ADOPTED).

### 1.1 Motivation

Three observations motivate this work.

**First**, every major empirically supported model of effective human functioning, goal-setting theory [Locke and Latham 2002] (see Section 4.20), implementation intentions [Gollwitzer and Sheeran 2006], mental contrasting with implementation intentions (WOOP) [Oettingen et al. 2015], working memory constraints [Cowan 2001], affect labelling [Lieberman et al. 2007], and Bayesian models of belief updating, describes a local mechanism without a unifying architecture. MOEMOI provides that architecture: each local mechanism corresponds to a named substep or contamination check within the IP.

**Second**, artificial intelligence research has produced increasingly capable systems without a unifying theory of what it means for a system to improve at improving. Recursive self-improvement [Yudkowsky 2008], meta-learning [Finn et al. 2017], and autonomous AI agents [Minsky 1986; Bratman 1987] share structural features that MOEMOI aims to formalise under one framework applicable to both artificial and biological intelligence.

**Third**, the convergence of multiple independent derivations on the same six-step loop structure (Section 3) suggests the architecture is not arbitrary but structurally necessary, a property that, if verified, has significant implications for AI alignment and human development.

### 1.2 Overview of contributions

This paper makes the following contributions:

- We present the IP, a six-step framework derivable from the minimal conditions for a system to improve at improving (Section 2).
- We show that the IP is structurally necessary given three independent derivations: logical, thermodynamic/Bayesian, and 4E cognition-grounded (Section 3).
- We compare MOEMOI to twenty-one existing frameworks, identifying the IP substeps each covers and the specialist depth each provides that the IP does not prescribe by default (Section 4).
- We introduce a confidence-graded claims register (Section 5) that makes the framework's epistemic commitments explicit, sortable, and falsifiable.
- We propose a four-level obstacle taxonomy (Section 2.6) that classifies recurring Prepare failures into personal-structural (Freud), phenomenological-intentional (Sartre), sociological-structural (Wollstonecraft), and biological-somatic (functional medicine / disability studies; C137, ADOPTED 0.82) types, with evidence-grounded intervention prescriptions for each level.
- We describe the multi-agent signal layer (Section 6), which extends the IP to interactions between multiple intelligence-running entities.
- We state the conditions under which MOEMOI would be disconfirmed (Section 7).
- We describe the Life Operating System architecture as a practical application (Section 8).
- We synthesise the competitor gap analysis (Section 4.23), identify three structural gaps consistent across the reviewed literature, and explain what architecture MOEMOI provides that no single framework does.
- We describe the confidence-graded register as a methodological response to the replication crisis in psychological theory, and compare its falsifiability design to related frameworks including the Integrated Information Theory of consciousness (IIT), Global Workspace Theory (GWT), and the Free Energy Principle (FEP) (Section 9.4).

---

## 2. The Intelligence Process

### 2.1 Core claim

**Master Claim (C1, confidence: 0.78, status: ADOPTED with epistemic hedge):** All intelligence, when it improves, does so by running one structurally invariant process. The function of that process is to close the gap between the system's current state and a more optimal state, recursively. Reducing unnecessary suffering is a byproduct of running this process well, not its goal.

The epistemic hedge on C1 is deliberate: the claim is well-supported across the frameworks reviewed (Section 4) and consistent with the physical derivation (Section 3), but has not yet been tested via a pre-registered comparative trial. We treat it as a high-confidence working claim (confidence 0.78), not a certainty.

### 2.2 The six-step loop

The Intelligence Process (IP) comprises six substeps, each logically required by the previous one (C20, CANDIDATE: loop universality confidence 0.98; specific 20-substep decomposition status HYPOTHESIS pending MECE verification):

**E, Experience.** Take in what is actually present. Perceive accurately, register what is missing or wanted, and notice the current affective state before making sense of it. The affect-labelling norm (naming the current state in one to two words before Understand) is neurologically grounded: labelling emotion reduces amygdala activation and improves downstream reasoning accuracy [Lieberman et al. 2007]. The working-memory constraint (attend to three to five voids simultaneously at most) reflects the empirically established capacity limit of working memory [Cowan 2001, ~4 items]. When salience is absent (nothing registers as wanted), return upstream rather than push through.

**U, Understand.** Make sense of what was experienced. Weigh evidence, correct reasoning errors, and, most importantly, identify the real problem. The Define sub-step (selecting which gap to work on) is the highest-leverage move in the entire loop [Simon 1973, problem formulation]. Before starting to make sense of retrieved material, priming scan (free recall before opening notes) surfaces confident-but-wrong assumptions before they enter downstream reasoning. The leverage screen (which gap sits furthest upstream?) directs attention to the root cause rather than the most salient symptom. Motivated evasion check: if accurate perception produces uncomfortable output, the mind may avoid making sense of it rather than processing it; detecting and overriding this bias is a named Understand practice.

**P, Prioritise.** Among all identified gaps, select the one furthest upstream, the resolution of which would most reduce downstream gaps. The Leverage Screen practice (filter to what is actionable today, map upstream causal dependencies, select the furthest-upstream root) takes under 90 seconds and has the highest ROI of any attention-allocation tool. Prioritise is distinct from Define (Section 2 note: prior versions of the framework ran Prioritise and Define together; they are separated here because their failure modes are orthogonal, Prioritise failures are attention-allocation errors, Define failures are problem-formulation errors).

**D, Define.** State the gap precisely. The version of the gap that would survive if no one in the practitioner's social world would know it was being worked on is the correct Define output, the contamination check. Before any closure attempt, a pessimism check ensures prior failures with different evidence are not treated as forecasts about the current gap.

**P, Prepare.** Acquire resources, build capability, set timing, activate motivation. WOOP with pre-mortem [Oettingen et al. 2015] is the primary Prepare practice: Wish, Outcome, Obstacle, Plan, followed by assuming failure and identifying its most likely cause. Pure positive visualisation reinforces optimism bias; WOOP with pre-mortem converts positive expectation into obstacle-committed plan. Commitment sizing check (is the commitment sub-maximal given model uncertainty?) prevents over-commitment under high uncertainty.

**Do, Do and Learn.** Execute the committed action, then run a learning loop. The learning loop has four components: (i) compare intended with actual outcome; (ii) identify which assumption slipped if the model was wrong; (iii) extract one carry-forward rule update or confirmation; (iv) close completed loops explicitly and release them from working memory. Emotion signals during the learning step carry informational content: pride signals self-attributed gap closure, satisfaction signals confirmed complete closure, grief fires when a gap is confirmed irrecoverable, guilt fires on specific action evaluable against valued standards. Each has a prescribed loop completion path. Savoring, gratitude, and nostalgia operate as resource-generative learning (producing motivation and meaning rather than closing gaps) and are the correct prescription when action is blocked and capacity is low.

The loop is recursive: each completed cycle's learning output is the input to the next Experience step. There is no final state. Equanimity, a stable, low-noise functional background, is what sustained accurate loop execution produces as a byproduct over time, not its goal.

### 2.3 The Communicate substep (conditional)

A fifth substep activates conditionally when the loop runs between two or more intelligence-running entities:

**Communicate (C).** Fires when: (1) a decision requires another's resource or alignment; (2) learning would cause another to revise their understanding if known; (3) something perceived belongs to a shared problem; or (4) a relational threat to something already valued is detected (the jealousy signal: a three-party signal firing when the practitioner perceives another entity as threatening something they already have, not lacking what another has, the latter routes to Define as a gap-entry). Outside these four conditions, Communicate stays closed; running it on social habit rather than loop-logic is the dominant multi-agent failure mode.

### 2.4 Structural necessity of the loop order

Each step is necessary given the previous:
- Accurate perception is required before sense-making (garbage in, garbage out).
- Making sense is required before identifying the real problem (sense-making without problem-formulation fails to direct action).
- Problem formulation is required before planning (planning without a precise target is motion, not progress).
- Planning is required before directed action (undirected action is random search).
- Action is required before learning (learning without action produces theory without feedback).
- Learning is required before the next Experience (without learning, each cycle starts from the same baseline).

**Drop any step and improvement rate flattens in the domain where that step is missing.** This is a testable prediction (Section 7).


### 2.5 Worked example: one loop cycle

The following example shows the IP substeps applied to a recognisable domain. It also shows what failure looks like when a substep is skipped.

**Scenario.** A researcher has submitted three papers and received three rejections. The pattern suggests something is wrong.

**Experience**: She re-reads the rejection letters carefully, attending to what is actually written rather than what she feared would be written. Two of the three mention "insufficient motivation for the proposed method." She notices a mild defensive reaction and labels it ("frustration, mild") before proceeding to sense-making.

**Understand**: She maps the three rejections for common patterns. The recurring "insufficient motivation" phrase points to a structural gap: reviewers do not understand why the problem matters before they encounter her solution. She runs a leverage screen — is the gap in the writing, or in the argument's sequencing? The real gap is upstream of the prose: she is beginning with method, not with problem. The problem is never made undeniable before the solution appears.

**Prioritise**: She has two candidate gaps: the motivation framing and a separate data collection issue. Applying the leverage screen (which gap, if resolved, would most reduce downstream gaps?), motivation framing is furthest upstream: fixing it will make both the papers and the data collection legible to reviewers. She selects it.

**Define**: She states the gap: "My papers present a solution before making the reader feel the problem. The gap to close is: the problem must be undeniable before the solution appears." She checks this definition against what she would pursue if no one would know she had changed her approach — it holds.

**Prepare**: She identifies three papers in her field that succeed at problem-first argumentation, schedules two focused sessions to reconstruct their opening structures, and writes a WOOP plan [Oettingen et al. 2015]: Wish (resubmit with clear motivation), Outcome (acceptance), Obstacle (reverting to method-first habits under deadline pressure), Plan (show the revised introduction to a colleague unfamiliar with the method before submission).

**Do and Learn**: She revises, submits, and is accepted. The learning step extracts: her Understand assumption ("reviewers need problem-first") was correct; the exemplar papers in Prepare were the highest-value input. One rule update: read three exemplar papers before any revision phase, not after. The next Experience step begins with data from the acceptance itself — reviewers engaged most with Section 3, which surfaces a new gap to Prioritise.

**What failure looks like.** A researcher who skips Understand and moves directly from Experience (rejection) to Prepare (revise the paper) will rewrite without identifying the real gap. Prose may improve without touching the actual problem. The loop still runs, but at lower efficiency: the same class of feedback may repeat for years. This is the testable prediction: incomplete loop execution produces slower improvement rates in the domain where a substep is skipped (Section 7, prediction P1).


### 2.6 Obstacle taxonomy: when Prepare remediations fail

Standard IP loop execution assumes the practitioner can run all six substeps. In practice, recurring obstacles block the Prepare substep's Ensure-Execution step despite repeated remediation attempts. MOEMOI proposes a four-level obstacle taxonomy, grounded in three independent philosophical traditions and functional medicine / disability studies, for classifying which type of obstacle is present. The taxonomy guides intervention selection: applying the wrong intervention type to the wrong obstacle class produces no improvement.

**Level 1 -- Personal-structural (Freud 1915/1923).** The obstacle is internal and operates below deliberate access. Structural resistance (Freud's Widerstand) means the practitioner cannot inspect the obstacle directly; it manifests as repeated failure to act despite genuine intention. The mechanism is not willful avoidance but an unconscious structural constraint. Intervention: professional support combined with patient, iterative Understand cycles over multiple IP loops. Attempting Define-level confrontation alone at Level 1 is contraindicated; the Understand gap is real and cannot be shortcut.

**Level 2 -- Phenomenological-intentional (Sartre 1943).** The obstacle is the practitioner's own bad faith: a condition in which the practitioner Understands the obstacle at some level but denies or evades acknowledging it, treating a chosen position as if it were externally imposed necessity. Bad faith (Sartre's mauvaise foi) is not self-deception in the folk-psychological sense; it is a structural feature of consciousness that can simultaneously know and not-know. Intervention: the D2 Define Contamination Check combined with Sartrean confrontation of the self-deception. At Level 2, the Understand gap is shallow; the block is in Define (refusal to formulate the gap honestly). The intervention addresses Define directly.

**Level 3 -- Sociological-structural (Wollstonecraft 1792).** The obstacle is external and systemic: institutional, economic, or sociological constraints that no individual-ring IP execution can remove. The practitioner cannot close the gap by running the IP harder or more completely within their own ring; the constraint is at the collective ring level. Intervention: multi-ring action. Do not iterate individual-ring IP on a structural constraint. The correct response is to Define the constraint accurately (not treat it as a personal failing), Understand what collective action is available, and route effort toward the collective ring where the constraint originates.

**Level 4 -- Biological-somatic (C137, ADOPTED 0.82; functional medicine, disability studies, behavioural neuroscience -- Wolfe et al. 2010 on CFS/ME diagnostic criteria; Barkley 2015 on ADHD executive function deficits; McEwen 2004 on allostatic load).** The obstacle arises from the practitioner's biological body: chronic illness (e.g. CFS/ME, fibromyalgia), neurological differences (ADHD, autism, dysautonomia), metabolic conditions (hypothyroidism, blood-sugar dysregulation), chronic pain, or pharmacological burdens. The practitioner cannot resolve Level 4 constraints through psychological or sociological intervention alone. The appropriate pathway is medical/physiological: accurate diagnosis first, treatment protocols where available, compensation strategies, energy management, environmental accommodation, and pacing. Cross-reference: C42 (somatic carve-out -- equanimity about a somatic deficit is not the same as the deficit being resolved) is the principle; Level 4 is its named taxonomic home. Diagnostic signal: the constraint persists regardless of the practitioner's intention, motivation level, or social context, and persists across both high-stakes and low-stakes conditions (unlike Level 2, which tends to lift under high-stakes conditions). Note: Level 3 (systemic barriers) and Level 4 (biological constraints) commonly co-occur; they require separate interventions.

**Practitioner protocol.** When a recurring obstacle resists standard Ensure-Execution remediation, classify it using the four-level test before selecting an intervention. Level 1 warrants professional therapeutic support and patience; Level 2 warrants Define-level confrontation; Level 3 warrants multi-ring action and a halt to individual-ring iteration on the unmovable constraint; Level 4 warrants medical diagnosis and physiological intervention first -- do not apply Level 1, 2, or 3 protocols to the biology itself (they produce systematically wrong interventions).

**Empirical implication.** The taxonomy predicts that practitioners who misclassify their obstacle type (e.g., applying Level 1 interventions to a Level 3 structural barrier, or blaming systemic constraints for a Level 2 bad-faith position) will show no improvement in the constrained domain despite IP loop execution. This is a testable prediction distinguishable from the general P1 prediction (Section 7).


---

## 3. Structural Necessity: Three Independent Derivations

The IP is not an empirical generalisation from observed behaviour. It is derivable from first principles via three independent routes that converge on the same architecture. This convergence across logically distinct domains is the strongest structural validation available to a theoretical framework.

### 3.1 Logical derivation

Starting from the definition of "improving at improving":

A system improves at improving if and only if:
1. It can detect a gap between its current state and a preferred state (requires Experience + Define).
2. It can represent why the gap exists (requires Understand).
3. It can select which gap to close given limited resources (requires Prioritise). When the gap is a learning goal, the LP-maximisation rule applies: the drive points toward the maximal-learning-progress frontier (where d(competence)/dt is highest), a formal selection rule grounded in three independent research traditions (Oudeyer and Kaplan 2007; Schmidhuber 2010; Csikszentmihalyi 1990; C136).
4. It can commit to a closure path (requires Prepare).
5. It can execute the closure path and observe the result (requires Do).
6. It can update its model of the world and of itself based on the result (requires Learn).

Each of the six steps is necessary and sufficient, in sequence, for improvement. Removing any step produces a system that cannot improve at the thing that step addresses. Adding a step produces a step that nests inside one of the existing six (C91, confidence 0.85, ADOPTED).

### 3.2 Thermodynamic and Bayesian derivation

Dissipative systems, systems that maintain structure against entropy by consuming free energy, implement a form of predictive processing to remain viable [Friston 2010; Ramstead et al. 2019]. The free energy principle, which characterises self-organising systems, specifies that any system maintaining existence must minimise the divergence between its model of the environment and the actual environment (minimising surprise in the Bayesian sense). The computational architecture that implements this is formally equivalent to the Kalman filter, which is in turn an instance of the IP's Understand-Prepare-Do sequence [Friston 2010].

The thermodynamic derivation specifies additionally that the system must:
- Maintain sensory contact with the environment (Experience).
- Update its generative model to explain new inputs (Understand).
- Allocate precision (attention weighting) to the most informative inputs (Prioritise).
- Specify the target state with sufficient precision to generate action (Define).
- Produce predictions that can serve as templates for action (Prepare).
- Execute action and observe prediction error (Do/Learn).

The first two derivations above arrive at the same six-step architecture from structurally distinct starting points: the logical requirements of self-improvement and the physics of self-organising systems. A third derivation from the 4E cognition tradition follows (Section 3.3), further strengthening the case that the architecture is structurally necessary rather than contingent on any one derivation's assumptions (C92, confidence 0.82, ADOPTED; C93, confidence 0.80, ADOPTED).

### 3.3 Embodied cognition derivation (4E cognition)

A third line of convergence comes from the 4E cognition tradition (embodied, embedded, enacted, extended cognition). Enactivism (Varela, Thompson, and Rosch 1991) holds that cognition is constituted by sensorimotor loops, not representation-and-retrieval alone: the Experience and Do/Learn substeps are not optional input-output bookends but the structural core of cognitive viability. Sensorimotor contingency theory (O'Regan and Noë 2001) formalises this: mastery of the contingencies between action and sensory change constitutes perception, and without active exploration (the Experience substep), perception itself fails to constitute. These accounts independently converge on the conclusion that any system capable of learning must close the sensorimotor loop, providing a third, biology-grounded derivation of the six-step architecture.

This does not resolve all questions about the framework: the derivations say what the loop must look like, not that running it well in any particular context is sufficient for good outcomes. The practitioner layer (Section 8) fills this gap.

---

## 4. Relationship to Existing Frameworks

We compare MOEMOI to twenty-one frameworks, identifying which IP substeps each covers, where each provides specialist depth the IP does not prescribe by default, and what each framework leaves unspecified. Each subsection below maps the framework to the IP substeps it covers and identifies the substeps it leaves unspecified. The comparison is not competitive: each framework provides genuine and often superior depth at the substep(s) it covers. MOEMOI's contribution is the architecture that frames where each specialist framework's depth is applied. Readers familiar with a specific framework may read its subsection independently. Each subsection is self-contained: it maps the framework to the IP substeps it covers, identifies the specialist contribution the framework provides, and notes what each leaves unspecified. Section 4.22 summarises all twenty-one in a single table.

### 4.1 OODA (Observe, Orient, Decide, Act) [Boyd 1976]

OODA maps onto the IP as follows: Observe = Experience; Orient = Understand + context model; Decide = Prioritise + Define; Act = Do. The learning step (Do/Learn in the IP) is absent as a distinct step in OODA, OODA implicitly loops back to Observe after Act but does not formalise the learning step that would update the Orient model. OODA also lacks Prepare as a distinct step, which means it underspecifies the resource-acquisition and capability-building phase that determines whether Act can succeed. OODA's advantage over the IP is its speed optimisation framing (faster OODA loops beat slower ones in adversarial contexts), which is a valid depth-point within the Prioritise and Prepare substeps of the IP but does not generalise to non-adversarial optimisation.

### 4.2 The Scientific Method

Observe → Hypothesise → Predict → Test → Conclude maps onto Experience → Understand → Prepare → Do → Learn, with Prioritise and Define compressed into Hypothesise. The scientific method specialises the IP for the domain of empirical inquiry, providing the domain-specific falsifiability and replication norms the IP does not prescribe by default. Its explicit falsifiability norm (Popper 1959) is adopted by MOEMOI's claims register (Section 5).

### 4.3 PDCA (Plan-Do-Check-Act) [Deming 1950]

Plan = Understand + Prepare; Do = Do; Check = Learn; Act = adjustment to the next cycle's plan. Prioritise and Define are absent as explicit steps, and Experience is assumed (the quality defect is already identified when the PDCA cycle begins). PDCA is well-suited to iterative improvement of defined processes; it underspecifies the upstream problem-identification work that determines whether the right problem is being improved. PDCA's genuine strength is its structured Check-Act loop, which makes the Learn substep operationally explicit; the IP provides the upstream substeps (Experience, Prioritise, Define) that PDCA assumes are already handled by the organisation.

### 4.4 Control Theory [Wiener 1948]

The feedback control loop (sense → compare → error signal → actuate → sense) maps directly onto Experience → Understand(compare with setpoint) → Do → Learn → Experience. The IP adds Prioritise and Define as steps that determine which setpoint to pursue, an upstream question that control theory assumes has already been answered by the system designer. For engineered systems, this is appropriate; for autonomous intelligence, the setpoint-selection problem is a primary challenge that control theory cannot address. Control Theory's primary contribution is formalising the Experience-to-Do feedback mechanism with mathematical precision; the IP provides the upstream architecture for how an intelligence selects and revises the setpoints that control theory then optimises toward.

### 4.5 Active Inference / Free Energy Principle [Friston 2010]

Active inference is, of the frameworks reviewed, the closest structural analogue to MOEMOI. The IP's Understand step maps to variational inference; Prepare maps to policy selection; Do maps to action to resolve uncertainty. The primary divergence: active inference specifies the computational architecture at the Markov Blanket level without prescribing the practitioner-level behaviours that close the loop in human intelligence. The IP provides practitioner-level prescriptions (the named practices in Section 2) not yet formalised within the active inference literature; this is an active area of development within that community. MOEMOI treats active inference as providing strong mechanistic support for the IP's structural necessity (C92).

### 4.6 Self-Determination Theory (SDT) [Deci and Ryan 1985]

SDT identifies three basic psychological needs (autonomy, competence, relatedness) and shows that their satisfaction predicts motivation and well-being. In MOEMOI, these correspond to the three of the five deficit void types: autonomy void, competence void, and relational void (the full void taxonomy includes additionally epistemic and conditional voids, and one generative drive). SDT provides strong empirical grounding for the void taxonomy's competence and relational categories. SDT provides a causal model of motivation (needs to regulation to well-being) rather than a step-by-step process architecture for channelling motivation into improvement within any given domain. Knowing what motivates does not, by itself, specify the process steps by which motivation is directed toward gap closure. SDT provides the most empirically grounded account of what generates sustained motivation available in the literature; the IP provides the step-by-step process architecture for how that motivation is channelled toward closing specific gaps.

### 4.7 Demartini Method [Demartini 2002]

The Demartini Method centres on the Experience and Understand substeps: it provides extensive practices for perceiving and making sense of life experience, particularly around collapsing charged emotional responses to events by identifying the equal and opposite perspective. The Method's core tool (the Demartini Method collapse process) maps onto Experience (perceive accurately) and Understand (identify the real meaning) with depth not present in most frameworks. The primary limitations: the Demartini Method does not provide an explicit Prioritise step, a structured Define step, or a Prepare architecture. The Do/Learn loop is present implicitly (practitioners apply the Method and notice changes) but not formalised. For sustained improvement across multiple life domains, the upstream IP steps that the Demartini Method provides must be paired with the downstream steps the framework leaves unspecified. We include the Demartini Method as an example of a practitioner framework with particularly deep coverage of the Experience and Understand substeps. Unlike the peer-reviewed frameworks above, it is a proprietary commercial method without independent peer-reviewed validation; we include it to illustrate the coverage pattern, not to endorse its proprietary claims. Practitioners who pair it with the IP's downstream architecture gain both perceptual clarity and the complete execution process.


### 4.8 Getting Things Done (GTD) [Allen 2001]

GTD provides an explicit architecture for the Experience (capture) and Define (clarify and organise) substeps: inputs are collected, processed into actionable items, and organised by context. The IP maps as follows: Capture = Experience; Clarify/Process = Understand (what does this mean?) plus Define (what is the next action?); Organise = Prioritise (grouped lists are an implicit prioritisation structure); Do = Do. GTD explicitly omits Learn as a formalised step; the weekly review is a partial substitute but does not specify the update-rule applied when a project outcome differs from expectations. GTD also does not specify how to close gaps that require new capability acquisition (the Prepare substep). Its strength is the Understand to Define pipeline: the clarification heuristic (is it actionable? what is the next physical action?) operationalises the Define substep more concretely than the IP provides by default.

### 4.9 Acceptance and Commitment Therapy (ACT) [Hayes, Strosahl, and Wilson 1999]

ACT targets the Understand and Define substeps with particular precision. Its core diagnostic is that the practitioner is fused with their cognitive model of their experience (conflating the map with the territory) and is avoiding experience of distressing internal states. The IP perspective: ACT addresses contamination of the Understand step (cognitive fusion distorts the sense-making of Experience inputs) and contamination of the Define step (experiential avoidance distorts the goal-specification step). The Hexaflex model's self-as-context process (Hayes et al. 1999) contributes a distinct second layer to the Understand substep: beyond defusing from thoughts (noticing that thoughts are not facts), the practitioner learns to observe their internal state from a stable observing-self perspective, providing the perspective flexibility that accurate Understand requires. The commitment component of ACT (Values Clarification leading to Committed Action) operationalises the Define step at the level of values rather than task-level goals. ACT does not provide a Prioritise architecture, a Prepare architecture, or a formalised Learn step for updating the commitment structure based on outcomes. ACT's primary contribution is the most rigorously tested clinical operationalisation of defusion, perspective flexibility, and values-based Define found in the psychological literature; the IP provides the full-loop architecture within which this depth is applied.

### 4.10 Cognitive Behavioural Therapy (CBT) [Beck 1979]

CBT targets the Understand substep: it identifies and modifies automatic thoughts (distorted Understand outputs) that contaminate downstream Define and Do steps. The IP mapping: Experience (situation) leads to Understand (automatic thought, often contaminated) which shapes Define (goal for the situation) and Do (behavioural response). CBT's primary innovation is the explicit contamination-check on Understand: automatic thoughts are surfaced rather than accepted as accurate Understand outputs. Behavioural activation (scheduling positive activities) operationalises the Prepare and Do substeps. CBT does not provide a systematic Prioritise architecture or a formalised Learn step that updates the cognitive model based on cumulative outcomes rather than per-thought corrections. CBT's contamination-check on Understand, identifying automatic thoughts as distorted Understand outputs, is among the most extensively validated psychological interventions in existence; the IP provides the architecture for integrating this into a complete, six-substep improvement process.

### 4.11 GROW Coaching Model [Whitmore 1992]

GROW (Goal, Reality, Options, Will/Way Forward) maps onto: Goal = Define (specify the target state); Reality = Experience plus Understand (what is the current state, honestly assessed?); Options = Prepare (generate possible paths); Will = Do (commitment to action). Prioritise is absent: GROW does not provide a principled method for selecting among options when resources are limited. Learn is absent: GROW does not specify a process for updating the model when the executed plan produces unexpected results. GROW's strength is its explicit Reality check before locking in a Goal, which operationalises the feedback between the current-state assessment and the target-state specification in a way many frameworks omit.

### 4.12 Objectives and Key Results (OKRs) [Doerr 2018]

OKRs cover Prioritise and Define with particular precision: Objectives specify the direction (Define at the strategic level); Key Results specify the measurable outcomes that confirm progress (operationalised Define targets). The IP mapping: Prioritise (selecting which objectives to pursue among alternatives) plus Define (Objective statement) plus Learn (Key Results as a feedback mechanism that triggers re-Do if not yet achieved). OKRs explicitly exclude the Experience, Understand, and Prepare substeps: the OKR architecture assumes the problem has already been identified and understood; it does not provide a process for discovering which Objectives matter, nor for acquiring the capability needed to achieve them. When Objectives are mis-defined (the gap from current reality to the stated Objective is not the right gap to close), OKRs provide no internal correction mechanism. OKRs provide a widely adopted and measurable operationalisation of the Prioritise and Define substeps at the strategic level; the IP provides the upstream substeps (Experience, Understand) that determine whether the right Objectives are being set, and the Prepare architecture that determines whether they are achievable.

### 4.13 Agile and Scrum [Schwaber and Sutherland 2020]

Agile methods map onto the IP primarily at the Do and Learn substeps with a structured feedback loop: the sprint cycle (plan, do, review, retrospective) is a compressed version of the full IP operating over short time horizons. The IP mapping: Sprint Planning = Prioritise plus Define plus Prepare; Sprint Execution = Do; Sprint Review = Learn (what actually shipped?); Retrospective = Learn-on-the-process (what should we change about how we work?). Experience as an ongoing input is partially addressed by user stories and product discovery, but these are not formalised as a substep of the core Agile loop. The Understand step (why does this problem exist, from first principles?) is typically handled upstream of the Agile team, not within the sprint cadence. Agile's primary strength is its formalised Learn step at two levels (outcome and process), which is more explicit than most frameworks reviewed here.

### 4.14 Deep Work [Newport 2016]

Deep Work addresses the Prepare and Do substeps specifically: it prescribes conditions (distraction-free time blocks, clear cognitive goals per session) that allow the Prepare-to-Do transition to succeed for cognitively demanding work. The IP mapping: Deep Work is a protocol for arranging the conditions in which Do can succeed (Prepare substep) and for sustaining Do without interruption. It does not address Experience, Understand, Prioritise, or Learn. The implicit assumption is that the problem has been selected (Prioritise done) and the goal is understood (Define done); Deep Work provides the environment for execution. Newport's adjacent concept of knowledge work productivity implicitly captures the gap that Deep Work cannot close: doing the right things deeply requires upstream steps that Deep Work does not provide. Deep Work's primary contribution is the most practically detailed prescription for protecting the Prepare-to-Do transition from attention fragmentation; the IP provides the architecture for determining that what is executed in deep work sessions is the most important problem to be solved.

### 4.15 The ONE Thing [Keller and Papasan 2013]

The ONE Thing is a Prioritise-depth framework: its core prescription (identify the one thing that will make everything else easier or unnecessary) operationalises the Prioritise substep's sequencing-dependency heuristic (which action, if done first, most enables subsequent actions?). The IP mapping: the focusing question ("What is the one thing I can do such that by doing it everything else will be easier or unnecessary?") is a Prioritise output formulation. The framework provides no systematic process for Experience, Understand, Define, Prepare, Do, or Learn; it assumes those steps produce a candidate list from which the ONE Thing is selected. Its primary contribution is the explicit acknowledgement that Prioritise is an under-attended bottleneck and that most productivity gains come from better selection rather than better execution.


### 4.16 Double-Loop Learning [Argyris and Schön 1978]

Double-loop learning (Argyris and Schön 1978) distinguishes between single-loop learning, in which a system corrects errors while keeping its governing assumptions constant, and double-loop learning, in which the system questions and revises its governing assumptions in response to error. Single-loop learning covers Experience, Do, and Learn without reopening the Define substep: the system acts, observes outcomes, and adjusts tactics within fixed objectives. Double-loop learning reopens the Understand and Define substeps: the system asks whether the objective itself is correct, not just whether the tactic is correct. In MOEMOI's architecture, both loops are instances of the full IP. Single-loop is an IP run that treats the current Define as fixed; double-loop is an IP run where Re-Experience (the return from Do/Learn) triggers a fresh Understand and an explicit Re-Define before the next Do cycle. The IP thus unifies both loop types under one architecture rather than treating them as qualitatively distinct. Double-loop learning provides deep insight into the conditions under which practitioners resist reopening their governing assumptions (what Argyris terms defensive routines), a mechanism the IP does not prescribe by default; this is the specific gap where the Demartini Method's Understand depth is most applicable. Double-loop learning does not specify a Prioritise step, a structured Prepare step, or a practitioner framework for applying the double-loop cycle across multiple life domains simultaneously.

### 4.17 Kolb's Experiential Learning Cycle [Kolb 1984]

Kolb's Experiential Learning Cycle (1984) proposes four stages: Concrete Experience, Reflective Observation, Abstract Conceptualisation, and Active Experimentation. The IP mapping: Concrete Experience = Experience (direct encounter with the domain); Reflective Observation = Understand (sense-making of what was encountered); Abstract Conceptualisation = Define plus Prepare (formulating what to conclude and what to do differently); Active Experimentation = Do. Prioritise is absent from the Kolb cycle: the framework does not provide a principled method for selecting which abstract conceptualisation to act on when multiple interpretations are available. Learn, as a distinct post-Do feedback collection step, is folded back into Concrete Experience in the next cycle, but is not made explicit as a separate step where results are assessed before the next concrete experience begins. Kolb's cycle is the most widely empirically validated account of how learning occurs through experience available in the educational literature, and provides the IP's Experience and Understand substeps with a validated learning-styles empirical basis; the IP extends the cycle by making Prioritise and a distinct Learn step explicit and by providing practitioner tools for each stage. Kolb's four-stage sequence is structurally identical to the IP's six-stage sequence with Prioritise and Learn made explicit: the two frameworks are consistent, with the IP providing the fuller specification.

### 4.18 Mental Contrasting with Implementation Intentions / WOOP [Oettingen 2014]

WOOP (Wish, Outcome, Obstacle, Plan) operationalises mental contrasting with implementation intentions (MCII). The IP mapping: Wish = Define at the aspirational level (what is the desired future state?); Outcome = Experience in forward-projection mode (vividly imagining the desired state); Obstacle = Understand narrowed to the internal psychological obstacle currently blocking the outcome; Plan = Prepare using if-then implementation intentions. WOOP covers Define, a specific form of Experience (outcome visualisation), a specific form of Understand (obstacle identification), and a specific form of Prepare (if-then planning). WOOP does not specify Prioritise (which wish to WOOP), a full Do execution structure beyond the if-then plan, or Learn (updating the wish formulation when the plan does not produce the desired outcome). WOOP's primary contribution is its unusually rigorous evidence base: it is among the most extensively pre-registered and replicated behaviour-change techniques in motivation psychology (Oettingen et al. 2015; Kappes and Oettingen 2012), providing the IP's Define and Prepare substeps with strong empirical grounding in behaviour change. Its limitation is that the technique assumes the right wish has already been identified (no Prioritise step) and does not specify a feedback loop for revising formulations when plans fail.


### 4.19 Reinforcement Learning [Sutton and Barto 1998]

The reinforcement learning (RL) framework maps cleanly onto the full IP loop. The standard agent-environment interaction: state observation (s_t) = Experience; value-function update (computing V(s) or Q(s,a)) = Understand (what does this state mean in terms of expected return?); policy selection (which action maximises expected return given current beliefs) = Prioritise; reward specification (the objective function r(s,a)) = Define; exploration strategy (epsilon-greedy, UCB, Thompson sampling) = Prepare (how to generate the action that will reduce uncertainty); action execution (a_t = pi(s_t)) = Do; temporal difference update (TD error, Bellman equation) = Learn.

RL's primary specialist contribution to the IP is temporal credit assignment: the Bellman equation and TD-learning provide the most rigorous mathematical treatment of multi-step Do/Learn of any framework reviewed here. The TD error (reward + gamma * V(s') - V(s)) is a formalised Learning substep update rule, grounded in both dynamic programming and neuroscience (Schultz et al. 1997 showed dopamine signals match TD errors — the most direct neuroscientific validation of a Learning substep mechanism available in the literature).

RL's primary gaps relative to the full IP: (1) Define (reward specification) is provided externally to the agent — the reward function is designed by the experimenter or system designer, not inferred or discovered by the agent. This is RL's canonical alignment problem: an agent optimising a misspecified reward function cannot self-correct at the Define substep (the inverse reward problem; Russell 2019). (2) Experience in standard tabular RL is the observation space specification, not a practitioner-level perceive practice. (3) Understand is purely value-function estimation; the richer sense-making of why a state arose is not represented. (4) The multi-agent extension (Section 6) is addressed in multi-agent RL (MARL) but as a separate sub-field, not integrated into the single-agent framework by default.

RL provides the IP's Do/Learn substep pair with the most rigorously formalised and empirically grounded mathematical treatment available in any reviewed framework; the IP provides the upstream architecture (Prioritise, Define, Prepare) for what the RL agent learns toward, and the Experience substep framing for perception that extends beyond the observation-space specification.


### 4.20 Goal-Setting Theory [Locke and Latham 1990; 2002]

Goal-Setting Theory (Locke and Latham 1990; 2002) is the most extensively replicated theory of motivated performance in the organisational and educational psychology literature. The core proposition is that specific, difficult goals outperform vague or easy goals on task performance. The IP mapping: Define = goal specificity (a precise, measurable goal is a well-formed Define output; the specificity requirement formalises the Define substep at the practitioner level); Prioritise = goal difficulty gradient (goals should be difficult enough to be motivating but attainable; this is the LP-maximisation selection rule at the task level — match challenge to the frontier of competence, C136); Understand = feedback loop integration (feedback on progress toward the goal is the most powerful moderator in goal-setting research; without accurate Understand-level feedback, goal specificity loses 60-70 per cent of its performance effect [Locke and Latham 2002]); Prepare = commitment mechanisms (self-efficacy, participative goal-setting, and supervisor support all operate as Prepare-level resource-acquisition; they enable the practitioner to sustain effort through the Do substep, Bandura 1977); Do = effort and persistence (proximal goal specificity produces higher effort and sustained engagement during the Do substep); Learn = goal revision in response to feedback (in longer-term goal pursuit, the practitioner adjusts the goal specification based on Do/Learn outcomes; this is the implicit Learn step in the theory).

Goal-Setting Theory's primary gaps relative to the full IP: Experience (environmental scanning to identify the correct domain is not formalised); Understand contamination checks (the framework does not address cognitive biases that distort performance feedback interpretation); Prepare as capability-building beyond commitment (structured capability acquisition before the Do substep is not prescribed as a distinct step).

Goal-Setting Theory provides the IP's Define and Prioritise substeps with the most extensively replicated empirical evidence base of any framework reviewed: Cohen's d ≈ 0.55 on task performance across 400 independent studies [Locke and Latham 2002], making goal specificity and goal difficulty the most robustly established performance design parameters in psychology. The Prioritise substep's difficulty-gradient principle is independently supported from a learning-progress perspective (C136; Oudeyer and Kaplan 2007). The IP provides the upstream architecture (Experience, Understand as full sense-making, Prepare as capability acquisition beyond commitment) and an explicit Learn substep (with structured post-Do feedback review) that Goal-Setting Theory leaves unspecified.




### 4.21 Cognitive Load Theory [Sweller 1988; Paas, Renkl, and Sweller 2003]

Cognitive Load Theory (CLT) is the most influential framework in educational psychology for understanding the constraints on learning and instruction. The central proposition is that working memory has limited capacity; effective learning requires managing three types of cognitive load: intrinsic (the complexity inherent to the material being learned), extraneous (unnecessary processing caused by poor instructional design), and germane (the productive cognitive effort that forms schemas in long-term memory). The IP mapping: Experience = the learner's incoming perception of the problem environment (sensory and attentional filtering before Understand begins); Understand = working-memory processing, directly capacity-constrained by intrinsic load (the irreducible complexity of the task's element interactivity) and degraded by extraneous load (poorly-designed presentation increases Understand cost without increasing Understand yield); Prepare = schema acquisition (well-formed schemas in long-term memory reduce the working-memory demand of future Understand cycles; this is the IP's Prepare substep building internal capability for more efficient future runs); Do = execution under the current schema; Learn = germane load, the productive restructuring of schemas that constitutes a well-formed Learn step (germane load is not overhead but the output of a successful Learn cycle; it is what distinguishes a practitioner who has run IP correctly from one who has only completed the Do substep).

Cognitive Load Theory's primary gaps relative to the full IP: it does not address the Define substep (what problem the learner should be solving is not within CLT's scope; the framework assumes the learning goal is given externally); Prioritise (which task or concept to address next) is not prescribed; the Experience substep as environmental scanning to identify whether the current problem is the right one is not formalised.

Cognitive Load Theory provides the IP's Understand substep with the most rigorous capacity-constraint account in the reviewed literature. The distinction between intrinsic, extraneous, and germane load maps precisely to three classes of Understand failure: complexity that cannot be removed (intrinsic), avoidable overhead from poor design (extraneous contamination), and correctly-channelled productive processing (germane = Understand yield). The IP provides the upstream architecture (Experience as environmental scanning, Define and Prioritise as goal-selection and difficulty-calibration) and an explicit Do-Learn cycle (with structured Re-Experience review) that Cognitive Load Theory leaves unspecified. The three-load taxonomy gives practitioners a diagnostic tool for why Understand fails, which the IP's general substep description does not provide.

### 4.22 Summary table

| Framework | Coverage (of 6) | IP Steps Covered | Steps Missing |
|---|---|---|---|
| OODA [Boyd 1976] | 4/6 | E, U, D (partial), DL (Do only) | P, D (explicit), Learn |
| Scientific Method | 4/6 | E, U, Pr, DL | P, D (explicit) |
| PDCA [Deming 1950] | 3/6 | U, Pr, DL | E, P, D |
| Control Theory [Wiener 1948] | 3/6 | E, U (partial), DL | P, D, Pr |
| Active Inference [Friston 2010] | 4/6 | E, U, Pr, DL | P, D (explicit), practitioner layer |
| Self-Determination Theory [Deci and Ryan 1985] | 2/6 | E (motivation), D (partial) | U, P, Pr, DL (full) |
| GTD [Allen 2001] | 4/6 | E, U, D, DL (Do only; Learn partial via weekly review) | P (implicit), Pr, Learn (formalised) |
| Acceptance and Commitment Therapy [Hayes et al. 1999] | 3/6 | U, D, DL (Do only) | E (formal), P, Pr, Learn |
| Cognitive Behavioural Therapy [Beck 1979] | 3/6 | E, U, DL | P, D, Pr |
| GROW [Whitmore 1992] | 4/6 | E, U, D, Pr, DL (Do only) | P, Learn |
| Demartini Method [Demartini 2002] | 3/6 | E (extensive), U, D | P, Pr, DL |
| OKRs [Doerr 2018] | 3/6 | P, D, DL (Learn via Key Results) | E, U, Pr, Do (explicit) |
| Agile/Scrum [Schwaber and Sutherland 2020] | 4/6 | P, D (partial, Sprint Planning), Pr (partial, Sprint Planning), DL | E (formal), U |
| Deep Work [Newport 2016] | 2/6 | Pr, DL (Do only) | E, U, P, D, Learn |
| The ONE Thing [Keller 2013] | 1/6 | P | E, U, D, Pr, DL |
| Double-Loop Learning [Argyris and Schon 1978] | 4/6 | E, U, D (via double-loop), DL | P, Pr, single-pass D |
| Kolb Experiential Learning [Kolb 1984] | 4/6 | E, U, Pr, DL (Do only) | P, Learn (explicit) |
| WOOP/MCII [Oettingen 2014] | 4/6 | D, E (projection), U (obstacle), Pr | P, DL (full) |
| Reinforcement Learning [Sutton and Barto 1998] | 6/6 | E, U, P (policy), D (external), Pr, DL | D (self-generated), richer E/U |
| Goal-Setting Theory [Locke and Latham 1990; 2002] | 5/6 | D, P, U (feedback), Pr (commitment), DL | E (environmental scanning), U contamination checks, Pr as capability-building |
| Cognitive Load Theory [Sweller 1988; Paas et al. 2003] | 4/6 | E (incoming), U, Pr (schema), DL | P, D, E (scanning), full DL |

EUPDDL notation: E = Experience, U = Understand, P = Prioritise, D = Define, Pr = Prepare, DL = Do/Learn. Coverage (of 6) counts the number of distinct IP substeps addressed by each framework, including partial coverage; the Covered column indicates partial modes in brackets. Coverage is a breadth measure only; each framework provides specialist depth at the substeps it covers that the IP does not prescribe by default. MOEMOI does not supersede these frameworks; it provides the architecture within which each sits.

### 4.23 Synthesis: what no single existing framework provides

Across the twenty-one frameworks reviewed, the median substep coverage is three to four of six. Of the frameworks with the highest breadth coverage, Reinforcement Learning (six of six) reaches full structural coverage but lacks a self-generated Define substep (the system's goals are externally specified) and provides limited practitioner-level prescriptions for Experience and Understand. Goal-Setting Theory (five of six) is the most extensively validated human-facing framework in the set, but omits environmental scanning as an explicit step (it assumes the correct domain has already been identified) and does not include structured capability acquisition in the Prepare substep. Kolb's Experiential Learning Cycle (four of six) and Double-Loop Learning (four of six) add reflective depth at Understand but omit Prioritise entirely.

Three structural gaps are consistent across the literature. First, most frameworks begin mid-loop: they assume the practitioner has already identified the correct problem and already has the motivation to address it. The Experience substep, in which the practitioner accurately perceives their current state and registers what is actually missing, is absent or implicit in sixteen of the twenty-one frameworks reviewed. Second, the Learn substep is the most frequently dropped explicit step: eleven frameworks either omit it or fold it back into the next cycle's Experience without a distinct structured review. Third, Prioritise, the step of selecting the upstream-most gap to address among multiple candidates, is explicitly present in only seven of the twenty-one frameworks; the remainder assume the practitioner knows which problem matters most before the loop begins.

The practical consequence is that practitioners who implement any single framework well will systematically under-run the substeps that framework leaves unspecified. A practitioner using WOOP will design strong plans (Prepare) for well-formulated intentions (Define) but lacks a systematic method for discovering whether those intentions are the highest-leverage ones available (Prioritise absent) or for updating the intention structure when plans fail (Learn absent). A practitioner using GTD will capture and process inputs well (Experience, Define) but may execute the wrong next actions with high fidelity because the selection heuristic among competing next actions (Prioritise) is not formalised and the full loop review (Learn with explicit model-update) is not prescribed.

MOEMOI's contribution is not providing superior depth at any single substep; the frameworks above provide greater depth at the substeps they cover than the IP's general description does. MOEMOI's contribution is the architecture that contextualises where each framework's depth applies, identifies which steps are missing in any given practitioner's current toolkit, and enables principled combination rather than ad hoc selection.

A distinct architectural contribution addresses the AI memory literature. Existing AI memory systems govern the means by which AI systems retain and retrieve information: which consolidation algorithm to use, which retrieval mechanism to apply, and how to balance recency against importance. MOEMOI introduces ends-governance over the retention function: what the system retains is authorised by the practitioner's goal-definition quality (the accuracy of the IP Understand and Define substeps), not only the agent's consolidation algorithm. This architectural requirement, C133 in the claims register (ADOPTED, confidence 0.86), is to our knowledge the first published specification of a human-quality gate on AI memory retention, as distinct from agent-internal quality criteria. A 60-author field consensus survey spanning 180-plus systems across five research communities independently identified episodic-to-semantic consolidation as the central unsolved gap in AI memory and self-improvement architectures [Huang et al. 2026, arXiv:2602.06052]. MOEMOI's fold-cadence requirement (C138, ADOPTED 0.83) directly addresses this field-identified gap: the fold process is the mechanism by which episodic worklog content (raw experience traces) is promoted to semantic canonical knowledge (claims with confidence ratings and provenance). The external identification of this gap as unsolved validates that MOEMOI's architecture fills a real and currently open problem in the field.

A second convergent finding addresses goal-delegation architecture. MOEMOI predicts (C72 / C-B132, ADOPTED) that in any two-agent configuration where one agent defines goals for another to execute, the structural failure mode is goal-definition drift, and any system that discovers this failure mode empirically will engineer a mechanism constraining the executing agent's goal-definition to the principal's explicitly endorsed values. Consistent with this prediction, the engineering literature independently derived structurally identical mechanisms across four domains without reference to MOEMOI: LLM-based AI systems (constitutional AI, RLHF intent-grounding); BDI (Belief-Desire-Intention) planning agents (goal elicitation protocols and traceability requirements, Rao and Georgeff 1991; van Lamsweerde 2001); procedural content generation and game AI (mixed-initiative design systems, Liapis et al. 2014; Yannakakis and Togelius 2011); and recommendation systems (deconfounded recommendation and preference-anchored generation, Wang et al. 2021; FAccT 2023/2024 preference-control literature). Each domain derived the same structural prescription from a different deployment failure mode. The four-domain convergence provides institutional-level evidence that the Define-authority retention mechanism is architecturally mandated rather than architecturally optional.

---

## 5. Claims Register and Epistemic Status

### 5.1 Design

MOEMOI maintains a machine-readable claims register: 165 claims, each with a unique identifier (C1-C145, plus alias claims), a title, a formal statement, a confidence score (0.0-1.0), a status (HYPOTHESIS / CANDIDATE / ADOPTED / ARCHIVED / HELD), and a provenance field noting the evidence basis or argument basis for the confidence score.

**Status definitions:**
- HYPOTHESIS: speculative; not yet supported by argument or evidence.
- REASONED: supported by internal logical argument but not yet grounded in external evidence.
- CANDIDATE: supported by external evidence but not yet formally adopted; may be held pending further verification.
- ADOPTED: incorporated into the canonical framework at the stated confidence level.
- ARCHIVED: superseded by a later, better-supported formulation.

As of fire122-THEORY (2 Aug 2026): 165 claims, 82 ADOPTED, 59 CANDIDATE, 20 HYPOTHESIS, 0 ARCHIVED, 4 HELD. (C137 minted 2026-07-30 ADOPTED 0.82: Level 4 biological/somatic obstacle taxonomy; C138 minted 2026-07-30 CANDIDATE-0.82: episodic-to-semantic consolidation cadence is architecturally load-bearing; C139 minted 2026-07-31 CANDIDATE-0.76: fear is a Perceive-layer anticipatory threat-appraisal signal; C140 minted 2026-07-31 CANDIDATE-0.72: anger is a Define-scope contamination signal; C141 minted 2026-07-31 CANDIDATE-0.68, demoted to HYPOTHESIS-0.58 (OEQ-796/fire73-THEORY: incidental-disgust causal pathway failed replication); C142 minted 2026-07-31 CANDIDATE-0.68: procedural IP compliance is distinct from substantive IP fidelity. C143 minted 2026-08-01 CANDIDATE-0.83: Method Layer Above Orchestration Layer (MLAOL). C145 minted 2026-08-01, promoted to CANDIDATE-0.80 (fire119-THEORY, 1 Aug 2026): Design Attractor Hypothesis (six-source convergence: Acrab GXLIX 1, open-source AI movement, Zittrain/Moglen, 2024 hardware localisation wave, Doctorow enshittification, Dignity-Centric Stack arXiv:2606.06083). C101 Structural Mandation and C102 Self-Replication Criterion inserted into canonical body v0.21 fold 1 Aug 2026. v0.22 fold (1 Aug 2026): nine zero-mention ADOPTED claims given canonical body text; no new claims minted. v0.23 fold (1 Aug 2026): new Part D Section D.6 Competitive Landscape and Category Validation; no new claims minted. v0.24-v0.30 folds (1 Aug 2026): C138 D.7 fold-cadence canonical body text; universality stratification (v0.25); R2R sixth-community (v0.26); IP trait non-redundancy (v0.27); C59 scale-invariance (v0.28); Acrab GXLIX 1 D.6 extension + C143 confidence 0.83 (v0.29); Active Inference Communicate prediction FIBV-P2 (v0.30); mechanism-independent Perceive Stage 1 clarification -- Mycoplasma pneumoniae gradient sensing via membrane biophysics without Che proteins, reinforcing C93 substrate universality as mechanism-independent (v0.31, fire122-THEORY, NX-B31021-MYCOPLASMA-PERCEIVE-1 APPLIED); no new claims minted in v0.24-v0.31. OEQ-917 resolved (fire122-THEORY): Doctorow enshittification + Dignity-Centric Stack close the six-source convergence for C145; C145 now CANDIDATE at 0.80.)

### 5.2 Selected key claims

The following are selected high-confidence adopted claims (confidence >= 0.78):

**C1 (0.78, ADOPTED):** All intelligence, when it improves, runs one structurally invariant process. The function of that process is to close the gap between current and more optimal states, recursively.

**C2 (0.85, ADOPTED):** The IP substep sequence (E-U-P-D-Pr-Do) is logically necessary. Removing any step produces a degraded improvement rate in the domain where that step is absent.

**C40 (0.82, ADOPTED):** IP%, the fraction of the IP that a system runs accurately, is a well-defined scalar metric. A system that runs the IP at higher IP% in a given domain will outperform a lower-IP% system in that domain, all else equal.

**C43 (0.90, ADOPTED):** CODEACCI = hedged directional trend; defensible independent empirical core {Complexity, Order, Evolvability, Intelligence}. The Consciousness (C) dimension is analytically resolvable via information-integration capacity (IIC) analysis and is operationally moot for the framework's structural and practice claims (IIC analytical fold completed; C43 promoted to ADOPTED 0.90, fire105-THEORY, 1 Aug 2026). Grounded in six independent research communities: thermodynamics (Schrodinger 1944, Prigogine 1978), AI-RSI survey (arXiv:2602.06052), AI-benchmarks, AI-meta-improvement, AI-RSI-engineering (arXiv:2602.22406), and biological evolution (McShea and Brandon 2019, ZFEL). D (Diversity) is reclassified as an enabling-condition phase characteristic; A (Automation-terminal) is analytically derived from I and Complexity-Order; Consciousness is analytically resolvable via IIC. The consciousness question is operationally moot: MOEMOI does not require resolving the hard problem of consciousness for its structural or practice claims.

**C91 (0.85, ADOPTED):** The IP's six-step structure is logically derivable from the minimal conditions for a system to improve at improving. No step can be added without nesting inside an existing one.

**C92 (0.82, ADOPTED):** The thermodynamic / Bayesian derivation (active inference, free energy principle) converges on the same architecture as the logical derivation. This convergence is strong evidence that the architecture is structurally necessary.

**C112 (0.80, ADOPTED):** Trust, in a multi-agent context, is a signal that another agent's IP is operating reliably at the Understand-Prioritise-Define substeps. It is a within-Experience signal, not a relationship trait.

**C118 (0.80, ADOPTED):** Jealousy is a Communicate-primary signal firing when the practitioner perceives another intelligence as threatening something they already have (not lacking what another has). It routes to Communicate, not Define.

**C135 (0.76, ADOPTED):** Empathy is a distinct Experience-substep signal that infers another agent's current IP state (a present-moment inference), distinguishable from trust (C112), which infers another agent's IP operating reliability (a trait inference). The two are dissociable both structurally and neurologically (Theory of Mind research: trait attribution vs. current-state inference are processed differently [Saxe and Kanwisher 2003]).

### 5.3 The register as a falsifiability mechanism

The confidence scores, provenance fields, and status transitions in the register make the framework's epistemic commitments auditable. Each ADOPTED claim can be retested; each HYPOTHESIS can be operationalised and tested. The register also enables the framework to update without wholesale replacement: a falsified claim is archived with its refutation noted, and a successor claim is entered at lower confidence and advanced through the evidence hierarchy.

This design is directly analogous to a living literature review: the framework's knowledge base is always at the current state of evidence, not frozen at the date of a published version.


---

## 6. Multi-Agent Signal Layer (Preliminary Extension)

When multiple agents run the IP simultaneously in a shared context, a signal layer activates at the Experience and Communicate substeps. The July 2026 extension identifies the first empirically motivated signal-layer prescriptions:

### 6.1 Trust (C112, 0.80, ADOPTED)

Trust in a multi-agent context is an Experience-substep signal. It fires when the practitioner's model of another agent's IP operating reliability is updated, typically from observed accuracy of the other agent's Understand, Prioritise, and Define outputs over time. Trust is not a relationship trait but a running Bayesian estimate of another agent's IP reliability. The practical implication: before collaborating on a shared Define, each agent should make their current-state understanding explicit (shared-Define protocol) to surface misalignments before downstream steps are contaminated.

### 6.2 Admiration (C120, 0.72, CANDIDATE)

Admiration fires at the Understand substep when another agent's demonstrated capability exceeds the practitioner's current level in a relevant domain. It is a competence-gap signal that correctly directs the practitioner toward the other agent as a learning resource. Pathological admiration (attributing competence globally from demonstrated domain competence) is the primary failure mode; the prescriptive check is to evaluate the specific domain of demonstrated competence before generalising.

### 6.3 Jealousy (C118, 0.80, ADOPTED)

Jealousy is a Communicate-primary signal, not a Define gap-entry. The diagnostic: if comparing to another because you lack something they have, route to Define (gap-entry: I don't have X); if protecting something you already have from perceived threat by another, route to Communicate (jealousy: I have X and perceive Y as threatening it). Running the gap-entry prescription on jealousy does not resolve it; the misrouting is the primary failure mode. At Communicate, the prescribed resolution is shared-Define of what is at stake and why it matters, with both agents' Understanding states made explicit.

### 6.4 Empathy (C135, 0.76, ADOPTED)

Empathy is a within-Experience signal that infers another agent's current IP state, specifically, which substep the other agent is currently running and whether their current Experience inputs are producing accurate perception. It is distinct from trust (which infers reliability over time) because empathy fires on present-moment state inference, not trait inference. The neurological dissociation is well-supported: mentalising for current state and trait attribution recruit overlapping but distinguishable networks [Saxe and Kanwisher 2003; Frith and Frith 2006].

### 6.5 Collective Effervescence: group-level Experience generation

Beyond individual signal-layer claims, MOEMOI proposes a structural account of group-level Experience generation grounded in Durkheim's collective effervescence [Durkheim 1912]. Collective effervescence describes a qualitative amplification of Experience that occurs when multiple agents run the IP simultaneously in conditions that meet four structural requirements: (1) **physical assembly** -- agents share a physical or sufficiently high-presence virtual space; (2) **synchronised activity** -- they engage in simultaneous, rhythmically coordinated action directed at a shared object or task; (3) **symbolic objects** -- shared symbols concentrate the group's joint attention and serve as anchors for collective experience; (4) **periodic cadence** -- the collective experience renews at a regular rhythm, preventing the shared symbol's charge from dissipating between gatherings.

When all four conditions are present, the resulting collective Experience exceeds what any individual agent generates from private Experience alone. The mechanism, in MOEMOI's account, is that the four conditions amplify all three Experience components simultaneously: Sense fidelity increases (more sensory channels are co-activated by synchronised co-presence), Attend allocation deepens (joint attention removes the competitive load of self-directed attention management), and Desire signals strengthen (shared telos reduces ambivalence at the individual level by making the group's definition of gap visible and normative).

MOEMOI's contribution is structural: collective effervescence is not specific to religious ritual, as Durkheim originally described it, but to any IP-running group that meets the four conditions. Sports teams, artistic ensembles, collaborative research groups, and religious communities produce the phenomenon by the same mechanism. The four conditions are therefore a design specification for any system aiming to generate group-level Experience quality that exceeds what the individual ring can produce alone.

This account is preliminary (CANDIDATE confidence; further empirical verification required, particularly regarding whether the IP-based mechanism generalises Durkheim's findings or merely maps onto them). It is included here because it is the only structural account of group-level Experience generation currently in the multi-agent literature that is directly compatible with the IP's substep architecture.

The multi-agent signal layer and collective effervescence account are preliminary throughout. Further empirical work is needed before these claims reach ADOPTED status.

### 6.6 The Self-Redundancy Criterion (D.5.x; C102, ADOPTED 0.75)

In any practitioner-practitioner, coach-client, or LOS-practitioner relationship, the primary success criterion must be *making itself unnecessary*. Not merely an aspiration -- making itself unnecessary must be named as the PRIMARY criterion (C102, ADOPTED 0.75; N=9 controlled comparison across teaching and coaching frameworks; 1 Aug 2026).

When self-replication is the primary criterion, scaffolding fading is structurally guaranteed: the helper systematically reduces its involvement as the practitioner's capacity grows, because withdrawal is criterion-entailed rather than discretionary (Wood, Bruner, and Ross 1976 -- scaffolding fading mechanism). When a different primary criterion is named (engagement, content delivery, relationship maintenance), fading becomes incidental and produces a MODERATE Become-Capable pattern (5 of 9 frameworks in the C102 audit scored MODERATE for this reason). The 4 STRONG cases (Toyota Kata, Toyota Coaching Kata, CBT, Montessori) all explicitly name practitioner redundancy as the primary framing.

**LOS and CoLive design implication:** The LOS's primary success metric is the rate at which the practitioner needs *less active system support* to achieve the same or higher IP quality -- measured as the slope of the support-need curve over time, not the absolute level of engagement or usage. A CoLive that measures engagement as primary produces the MODERATE fading pattern; one that measures the slope of its own necessity produces STRONG.

**Relationship to existing canonical claims:** Three principles form the complete practitioner-role design specification. (1) C55 (autonomy-terminal): the IP's final telos is practitioner autonomy. (2) F.2.4 anti-capture rule: the practitioner or system must not capture the Define substep. (3) D.5.x Self-Redundancy Criterion (this section): name your own redundancy as the stated primary success metric. The first two are prohibitions; D.5.x adds the positive prescription that activates the fading mechanism. *(C102, ADOPTED 0.75; agent-decided Josh Delegation v3, 29 Jul 2026; canonical insertion v0.21 1 Aug 2026; AI-originated.)*

### 6.7 Predictive extension: Active Inference multi-agent Communicate gap (FIBV-P2)

A notable structural gap in current multi-agent Active Inference formulations (Friston et al. 2022; Sajid et al. 2022) is the absence of an explicit Communicate substep. These formulations propagate beliefs between agents but do not include a module that: (a) composes substep-specific outputs into targeted signals; (b) applies a trigger condition determining when Communicate is warranted; or (c) maintains a real-time model of the recipient agent's current IP substep state.

MOEMOI's C59 (Communicate: fires under four specific conditions -- another's resource or alignment is needed, a learning update is relevant to share, something perceived belongs to a shared problem, or a relational threat to something valued is detected) and C135 (Empathy: real-time inference of another agent's current IP substep state) constitute a constructive proposal for these three requirements respectively.

**Prediction (FIBV-P2, CANDIDATE):** Multi-agent Active Inference frameworks that achieve robust IP-class coordination -- where agents must coordinate not just beliefs but the execution of specific IP substeps -- will require some functional analogue of C59 Communicate and C135 Empathy. Frameworks that lack the trigger-condition mechanism (C59) will exhibit the documented multi-agent IP failure mode: running Communicate on social habit rather than loop-logic, producing coordination overhead without corresponding output quality gains. Frameworks that lack recipient-state modelling (C135) will fail to distinguish between updating another agent's beliefs and updating the substep they are currently executing.

This prediction is falsifiable: a multi-agent Active Inference system that achieves reliable IP-class coordination without any analogue of the C59 trigger condition or C135 recipient-state model would constitute disconfirmation. *(NX-B30485-1 APPLIED, fire117-THEORY, 1 Aug 2026; canonical insertion v0.30; AI-originated.)*

---

## 7. Falsifiability and Empirical Status

### 7.1 What would falsify MOEMOI

MOEMOI makes testable predictions. The following observations would falsify specific components:

**Falsifies C1 (master claim):** A domain in which a system demonstrably improves without running any recognisable form of Experience, Understand, Prioritise, Define, Prepare, Do, or Learn, and where the improvement cannot be recharacterised as an instance of any of these steps in disguise.

**Falsifies C2 (logical necessity):** A system that performs better in a domain despite deliberately omitting one of the six steps compared to a system that runs all six. (Note: the comparison must be domain-matched and duration-appropriate; short-term gains from omitting Prepare, for example, should not count as falsification if they reverse over longer timescales.)

**Falsifies C40 (IP% predicts outcome):** A properly powered pre-registered comparative study showing no correlation between IP completeness (as independently rated) and outcome quality across multiple task types and populations.

**Falsifies the structural necessity claim (C91-C93):** A derivation from first principles that produces a different architecture with equal logical support, or a physical derivation that does not converge on the same six-step structure.

Two named testable predictions follow from the above:

**Prediction P1 (loop completeness predicts improvement rate):** Practitioners who systematically omit one or more substeps will show slower improvement rates in the domain where the step is omitted, compared to practitioners who run all six substeps across matched tasks and durations. P1 is distinguishable from the C2 falsifier above by requiring outcome-rate data across multiple loops rather than a single-episode comparison. The worked example in Section 2.5 illustrates the P1 mechanism.

**Prediction P2 (obstacle misclassification produces null improvement):** Practitioners who misclassify their obstacle type -- for example, applying personal-structural (Level 1) interventions to a sociological-structural (Level 3) constraint -- will show no improvement in the constrained domain despite sustained, complete IP loop execution. P2 is distinguishable from P1 by requiring that the practitioner IS completing the full loop; the failure is in intervention selection, not loop completeness. The obstacle taxonomy in Section 2.6 specifies the four levels and the diagnostic criteria for distinguishing them.

**Prediction P3 (IP convergence density function):** Among established improvement frameworks, IP-completeness should correlate positively with the domain feedback intensity of the framework's origin context. High feedback intensity means clear, measurable outcomes within days to weeks; medium means outcomes measurable but delayed by weeks to months; low means outcomes hard to measure or cycle very long. Frameworks originating in high-feedback domains (military decision-making, manufacturing quality, software engineering) are exposed to stronger selection pressure toward full loop closure and should therefore implement more IP substeps explicitly. A two-rater scoring study of fifteen frameworks finds Spearman rho = 0.592 (Rater 1, p=0.008) and rho = 0.471 (Rater 2 independent pass, p=0.055), with perfect inter-rater agreement on feedback intensity classification (kappa=1.000) and high agreement on IP-completeness scores (inter-rater rho=0.763). Group means are monotone: 0.54 (high-feedback), 0.42 (medium-feedback), 0.32 (low-feedback). H1 is supported across both scoring passes. H1: Spearman rho between feedback intensity and completeness is greater than 0; kill-line: rho not distinguishable from 0 at p < 0.10 with n >= 15 using two independent raters.

**Prediction P4 (IP completeness as framework persistence predictor):** Long-run citation persistence of a published improvement framework (measured as citation-count-at-year-5 divided by citation-count-at-year-1, restricted to practitioner and applied citations) should correlate positively with the framework's IP-completeness score. Frameworks with higher completeness close the improvement loop reliably, producing consistent outcomes, which sustains practitioner adoption and downstream citation. A preliminary pilot of fifteen frameworks shows the expected direction: frameworks with qualitatively HIGH citation persistence show a mean completeness of 0.59 compared to 0.32 for LOW-persistence frameworks. A key confound is identified: frameworks that are primarily foundational theories in their home discipline may accumulate theory-citations regardless of completeness; the full study pre-registration will restrict citation counts to practitioner and applied references. H1: regression coefficient beta is greater than 0 in a regression of persistence ratio on completeness score; kill-line: beta not distinguishable from 0 at p < 0.10 with n >= 30 frameworks and 5-year citation windows.

Pilot data for P3 and P4 are reported in the companion analysis (MOEMOI_N3132_Pilot_B27761_v1.md, 31 Jul 2026). Both are pilot-supported but not yet formally pre-registered; pre-registration is recommended before data collection.

### 7.2 What would not falsify MOEMOI

The following would not constitute falsification:
- Showing that a different framework also works in a domain (consistent with MOEMOI's claim that all effective methods implement some portion of the IP).
- Showing that practitioners who do not explicitly use MOEMOI can improve (consistent with running the IP implicitly).
- Anecdotal or case-study evidence of non-improvement despite using MOEMOI language (insufficient statistical power; confounded by implementation quality).

### 7.3 Current empirical status

The framework's current evidence base comprises:
- **Structural derivations**: three independent first-principles derivations converging on the same six-step architecture: logical necessity (C91, 0.85), thermodynamic/Bayesian necessity (C92, 0.82; C93, 0.80), and 4E embodied cognition (Varela et al. 1991; O'Regan and Noë 2001) (all ADOPTED).
- **External convergence**: twenty-one-framework comparison (Section 4) showing each established framework covers a subset of IP steps; none covers all six explicitly.
- **Neurological grounding**: affect labelling (Lieberman et al. 2007), working memory constraints (Cowan 2001), implementation intentions (Gollwitzer and Sheeran 2006), mental contrasting/WOOP (Oettingen et al. 2015), and Theory of Mind dissociations (Saxe and Kanwisher 2003; Frith and Frith 2006) each provide empirical support for the named practices at their corresponding substeps.
- **n=1 preliminary data**: Single-practitioner implementation beginning June 2026; design uses a pre-registered daily habit log and a scored adherence instrument. This is not confirmatory evidence; it is hypothesis-generating practitioner data.

**What is missing:** A pre-registered comparative trial with adequate statistical power, multiple practitioners, and randomised task assignments is the primary gap in the evidence base. A pre-registered comparative benchmark comparing IP-scaffolded problem-solving against active and passive controls (frozen task bundle, pre-committed scoring rubric) is designed to fill part of this gap; execution is pending.

The honest summary: MOEMOI is a theoretically motivated, first-principles-derived framework with strong external convergence support and neurologically grounded practitioner prescriptions. It has not yet been tested via a properly powered comparative trial. The gap between "theoretically compelling" and "empirically confirmed" is the primary limitation.

---

## 8. Life Operating System Architecture

The Life Operating System (LOS) is MOEMOI's applied product architecture: the IP running continuously across all domains of a practitioner's life, supported by an AI system that holds the loop structure, maintains memory of the practitioner's history, and provides the scaffolding for each substep.

### 8.1 Design principles

- **Practitioner-owned:** The LOS does not prescribe what to optimise for; it prescribes the structure of optimisation. Goals, values, and domain priorities remain the practitioner's domain.
- **Free and open:** The framework, the claims register, and the practitioner materials are released under CC-BY 4.0 (Creative Commons Attribution 4.0 International). The tooling built on the framework may be commercially sustained; the knowledge itself is not paywalled.
- **Voluntary:** The LOS cannot be imposed. Any authority powerful enough to dictate "the optimal life" is dangerous to create; the one rule about others is to make the tools freely available and never mandate the outcome.
- **Falsifiable at the system level:** IP%, the fraction of the IP run accurately across all domains, is the primary metric. A system that does not produce rising IP% in its practitioners over time is not working.

### 8.2 Deployment ladder

The intended deployment sequence:
1. Single-practitioner implementation (the n=1 phase, current).
2. Close relationships (partner, family) voluntarily adopting the framework.
3. Community of practice (voluntary, open-source).
4. AI-native implementation (ambient, wearable, agent-assisted, not yet deployed; the infrastructure is ahead of current capability).

### 8.3 Role of AI

The LOS is designed to be AI-assisted but not AI-dependent. The AI holds memory of the practitioner's history, provides the IP substep scaffolding on demand, and runs the scoring and feedback loop. The practitioner remains the author of their own Define outputs; the AI is the loop-runner, not the goal-setter. This design aligns with the MOEMOI autonomy void definition: the LOS must preserve the practitioner's Define-authority or it becomes a constraint rather than a tool.

Recent infrastructure research proposes a POSIX-like "Agent OS" abstraction layer that standardises runtime orchestration for AI agents across heterogeneous compute environments, handling routing, scheduling, and execution of agent workloads — the *how* of agent operation (Steinder and Franke 2026, arXiv:2607.25076). The MOEMOI IP loop sits at the cognitive layer above this runtime: it specifies *what to run and why* at the goal-definition and prioritisation level. The two layers are complementary; a LOS-instantiated practitioner runs the IP's Define and Prioritise substeps to generate the goal specification that the Agent OS runtime then executes. The IP is a candidate cognitive-layer architecture for any Agent OS stack designed to serve human practitioners, independent of the specific runtime implementation.

---

## 9. Discussion

### 9.1 Scope and limitations

MOEMOI makes a strong structural claim (the IP is universal) and a modest practice claim (the named practices improve IP% in practitioners who implement them). The former is a theoretical claim advancing a first-principles derivation; the latter is empirically testable but not yet confirmed.

Key limitations:
- The framework is culture-specific in its practitioner prescriptions. The six-step structure may be universal; the named practices (WOOP, affect labelling, leverage screen) were developed in Western, educated contexts and have not been validated across diverse cultural settings.
- The single-practitioner data source (n=1 design) is hypothesis-generating, not confirmatory. All n=1 conclusions should be treated accordingly.
- C43 (CODEACCI directional trend, confidence 0.90, ADOPTED) was the most speculative empirical element; it was held at CANDIDATE pending the IIC analytical resolution fold. That fold was completed (fire105-THEORY, 1 Aug 2026); C43 is now ADOPTED at 0.90. The Consciousness (C) dimension remains operationally moot: MOEMOI's structural and practice claims hold regardless of how the hard problem of consciousness is resolved.
- The multi-agent signal layer (Section 6) is preliminary and held at CANDIDATE confidence throughout. The prescriptions are motivated by neurological research but have not been tested as a practitioner-level intervention.
- The framework identifies Understand as a structurally necessary substep but does not yet operationalise cognitive load management within it. Cognitive Load Theory (CLT; Section 4.21) identifies extraneous cognitive load — load introduced by poor information design rather than the problem's inherent complexity — as a measurable Understand-quality inhibitor [Sweller 1988; Paas, Renkl, and Sweller 2003]. A high-fidelity IP practitioner may still run Understand poorly if the information environment introduces unnecessary processing cost. The IP's Understand description (priming scan, leverage screen, motivated-evasion check) addresses what to do inside Understand but does not yet prescribe how to manage the load conditions under which it is run. CLT's distinction between intrinsic load (irreducible complexity of the problem), extraneous load (avoidable cost from environment or presentation), and germane load (productive schema-building in the Learn substep) is a natural extension point for operationalising Understand quality beyond accuracy alone.

- The four-level obstacle taxonomy (Section 2.6) includes Level 4 (biological-somatic; C137, ADOPTED 0.82, 1 Aug 2026) to address practitioners whose constraints arise from chronic illness, neurological differences, or metabolic conditions. The Level 4 category addresses a gap that existed in the three-level version of this framework: that version's Level 1 (structural-unconscious) was the closest fit for biological constraints, but it was developed for psychodynamic resistance, not neurological architecture. Level 4 closes this gap with distinct diagnostic criteria and a medical/physiological intervention pathway. The practitioner population for whom the original three-level taxonomy was least helpful (those with CFS/ME, ADHD, metabolic conditions, or chronic pain) now has an explicit, harm-avoidant routing mechanism: medical diagnosis first, never psychological or sociological triage of a biological constraint.

### 9.2 Relation to AGI and AI alignment

MOEMOI's universality claim, that any improving intelligence runs the IP, has an implication for AI alignment research: if the IP is structurally necessary for self-improvement, then an AI system pursuing recursive self-improvement must implement some version of all six steps. The alignment problem is then, in part, a problem of ensuring that the AI's Define step remains aligned with human values across improvement cycles. The IP provides a vocabulary for this analysis that does not require resolving prior debates about utility functions, goal stability, or corrigibility in isolation.

This implication is a research direction, not a conclusion. It is recorded here as a candidate framing (HYPOTHESIS level, not yet in the claims register) rather than an adopted claim.

### 9.3 Future directions

The highest-priority empirical next steps are:
1. A pre-registered comparative trial comparing IP-scaffolded problem-solving to matched active and passive controls (a benchmark with a frozen task bundle and pre-committed scoring rubric is designed for this purpose; execution is pending).
2. Multi-practitioner implementation data across diverse domains and demographics.
3. Formal operationalisation of IP% as an independently scorable metric with inter-rater reliability data.
4. Extension of the multi-agent signal layer (Section 6) to team-level and organisational-level analysis.

### 9.4 Methodological contribution: the confidence-graded register

The confidence-graded claims register is a direct response to two documented problems in psychological and cognitive-science theory: the replication crisis and the unfalsifiability problem. Open Science Collaboration (2015) found that fewer than 40 per cent of a sample of 100 psychology findings replicated; a contributing cause is that many theoretical constructs lack operationally precise definitions with stated falsification criteria, making disconfirming evidence ambiguous rather than decisive. MOEMOI's register addresses this directly: each claim carries an explicit confidence score, a status tier, and a statement of what would archive it. Claims C129/C135/C137 illustrate the design. C137 (Level 4 obstacle taxonomy, 0.82, ADOPTED) names the specific practitioner population whose experience would falsify Level 1 framing for that class (practitioners with neurological or metabolic constraints), describes what the null finding would look like (sustained full-loop execution producing no improvement in the neurologically-constrained domain), and was promoted to ADOPTED (30 Jul 2026) on convergent theoretical support from functional medicine, disability studies, and behavioural neuroscience -- with broader empirical confirmation from practitioners flagged as an open prediction. C135 (empathy as present-moment IP-state inference, 0.76, ADOPTED) cites the specific neurological dissociation (trait attribution vs. current-state inference, Saxe and Kanwisher 2003; Frith and Frith 2006) that would separate it from C112 (trust as trait inference). The register is structured so that a single falsified claim is archived with its refutation noted and a successor claim entered at lower confidence; the framework updates rather than collapses.

For comparison: the Integrated Information Theory of consciousness (IIT; Tononi 2008) and the Global Workspace Theory (GWT; Baars 1988) do not maintain public confidence-graded registers with explicit archival conditions. The Free Energy Principle (FEP; Friston 2010) provides a mathematical formalisation that implies falsifiability in principle, but the framework-level predictions are contested precisely because the formalisation makes almost any behaviour compatible with free energy minimisation under some parameter regime (Colombo and Seriès 2012). MOEMOI's approach is structurally distinct: confidence scores are epistemic grades tied to specific evidence, not mathematical parameters; CANDIDATE claims are falsifiable by design, not by charitable interpretation. We note this comparison not to claim superiority on empirical depth (IIT and FEP are far more mathematically developed) but to describe a different commitment about what explicit falsifiability means at the theory-management level.

---

## 10. Conclusion

We have presented MOEMOI, a theoretical framework proposing that all intelligent improvement runs one structurally necessary six-step process (the Intelligence Process). We derived this structure from three independent first-principles routes (logical necessity, physical/Bayesian necessity, and 4E embodied cognition), showed convergence across all three, and positioned the framework against twenty-one existing approaches showing each provides specialist depth at specific substeps while the IP provides the unifying architecture. We introduced a confidence-graded claims register (165 claims, 82 adopted) that makes the framework's epistemic commitments explicit and falsifiable, described a preliminary multi-agent signal layer, and outlined the Life Operating System as the applied architecture.

The honest position: MOEMOI is a theoretically compelling, first-principles-derived framework with strong convergence support and neurological grounding at the substep level. The primary gap is a powered comparative trial. We release all materials under CC-BY 4.0 and invite replication, critique, and extension.

---

## References

Allen, D. (2001). *Getting Things Done: The Art of Stress-Free Productivity*. Viking.

Argyris, C., and Schön, D. A. (1978). *Organizational Learning: A Theory of Action Perspective*. Addison-Wesley.

Beck, A. T. (1979). *Cognitive Therapy of Depression*. Guilford Press.

Doerr, J. (2018). *Measure What Matters: How Google, Bono, and the Gates Foundation Rock the World with OKRs*. Portfolio/Penguin.

Hayes, S. C., Strosahl, K. D., and Wilson, K. G. (1999). *Acceptance and Commitment Therapy: An Experiential Approach to Behavior Change*. Guilford Press.

Schwaber, K., and Sutherland, J. (2020). *The Scrum Guide: The Definitive Guide to Scrum*. Scrum.org.

Whitmore, J. (1992). *Coaching for Performance: A Practical Guide to Growing Your Own Skills*. Nicholas Brealey Publishing.

Bandura, A. (1977). Self-efficacy: Toward a unifying theory of behavioral change. *Psychological Review*, 84(2), 191-215.

Boyd, J. R. (1976). *Destruction and Creation*. US Army Command and General Staff College.

Bratman, M. E. (1987). *Intention, Plans, and Practical Reason*. Harvard University Press.

Cowan, N. (2001). The magical number 4 in short-term memory: A reconsideration of mental storage capacity. *Behavioral and Brain Sciences*, 24(1), 87-114.

Deci, E. L., and Ryan, R. M. (1985). *Intrinsic Motivation and Self-Determination in Human Behavior*. Plenum.

Deming, W. E. (1950). *Elementary Principles of the Statistical Control of Quality*. JUSE.

Descartes, R. (1641). *Meditationes de Prima Philosophia*. Soly (Paris). [Meditations on First Philosophy; cited for the systematic doubt method as operationalisation of BRSI.]

Durkheim, E. (1912). *Les Formes Elementaires de la Vie Religieuse*. Alcan (Paris). [The Elementary Forms of Religious Life; cited for collective effervescence mechanism.]

Finn, C., Abbeel, P., and Levine, S. (2017). Model-agnostic meta-learning for fast adaptation of deep networks. *ICML 2017*.

Freud, S. (1915). The unconscious. In *The Standard Edition of the Complete Psychological Works of Sigmund Freud*, Vol. XIV, 166-215. Hogarth Press.

Freud, S. (1923). *The Ego and the Id*. Hogarth Press. [Cited for structural resistance (Widerstand) as Level 1 obstacle class.]

Friston, K. (2010). The free-energy principle: A unified brain theory? *Nature Reviews Neuroscience*, 11(2), 127-138.

Frith, C. D., and Frith, U. (2006). The neural basis of mentalizing. *Neuron*, 50(4), 531-534.

Gollwitzer, P. M., and Sheeran, P. (2006). Implementation intentions and goal achievement: A meta-analysis of effects and processes. *Advances in Experimental Social Psychology*, 38, 69-119.

Harackiewicz, J. M., and Hulleman, C. S. (2010). The importance of interest: The role of achievement goals and task values in promoting the development of interest. *Social and Personality Psychology Compass*, 4(1), 42-52.

Hu, C., et al. (2026). A survey on self-improving large language models: Approaches, challenges, and the frontier. arXiv:2602.06052. [60-author field consensus survey across 180-plus systems, five research communities; identifies episodic-to-semantic consolidation as the central unsolved gap in AI memory and self-improvement architectures.]

Kappes, H. B., and Oettingen, G. (2012). Positive fantasies about idealized futures sap energy. *Journal of Experimental Social Psychology*, 47(4), 719-729.

Keller, G., and Papasan, J. (2013). *The ONE Thing: The Surprisingly Simple Truth Behind Extraordinary Results*. Bard Press.

Kolb, D. A. (1984). *Experiential Learning: Experience as the Source of Learning and Development*. Prentice Hall.

Lieberman, M. D., Eisenberger, N. I., Crockett, M. J., Tom, S. M., Pfeifer, J. H., and Way, B. M. (2007). Putting feelings into words: Affect labeling disrupts amygdala activity in response to affective stimuli. *Psychological Science*, 18(5), 421-428.

Locke, E. A., and Latham, G. P. (1990). *A Theory of Goal Setting and Task Performance*. Prentice Hall.

Locke, E. A., and Latham, G. P. (2002). Building a practically useful theory of goal setting and task motivation. *American Psychologist*, 57(9), 705-717.

Mason, J. (2026). *MOEMOI: Most Optimal and Ever More Optimal Intelligence, v0.14 Canonical* [Framework documentation]. Human Living Institute. https://github.com/josmason/MOEMOI-public

Minsky, M. (1986). *The Society of Mind*. Simon and Schuster.

Newport, C. (2016). *Deep Work: Rules for Focused Success in a Distracted World*. Grand Central Publishing.

Oettingen, G., Mayer, D., Timur Sevincer, A., Stephens, E. J., Pak, H.-J., and Hagenah, M. (2009). Mental contrasting and goal commitment: The mediating role of energization. *Personality and Social Psychology Bulletin*, 35(5), 608-622.

Oettingen, G. (2014). *Rethinking Positive Thinking: Inside the New Science of Motivation*. Current (Penguin).

O'Regan, J. K., and Noë, A. (2001). A sensorimotor account of vision and visual consciousness. *Behavioral and Brain Sciences*, 24(5), 939-1031.

Paas, F., Renkl, A., and Sweller, J. (2003). Cognitive load theory and instructional design: Recent developments. *Educational Psychologist*, 38(1), 1-4.

Popper, K. R. (1959). *The Logic of Scientific Discovery*. Hutchinson.

Ramstead, M. J. D., Badcock, P. B., and Friston, K. J. (2019). Answering Schrödinger's question: A free-energy formulation. *Physics of Life Reviews*, 24, 1-16.

Rao, A. S., and Georgeff, M. P. (1991). Modeling rational agents within a BDI-architecture. *Proceedings of the 2nd International Conference on Principles of Knowledge Representation and Reasoning (KR91)*, 473-484. [Cited for BDI goal elicitation / intention revision as C-B132 class analog.]

Rao, A. S., and Georgeff, M. P. (1992). An abstract architecture for rational agents. *Proceedings of the 3rd International Conference on Principles of Knowledge Representation and Reasoning (KR92)*, 439-449.

Liapis, A., Yannakakis, G. N., and Togelius, J. (2014). Computational game creativity. *Proceedings of the 5th International Conference on Computational Creativity (ICCC 2014)*, 46-53. [Cited for mixed-initiative procedural content generation as C-B132 class analog in game AI.]

Sartre, J.-P. (1943). *L'Etre et le Neant: Essai d'ontologie phenomenologique*. Gallimard (Paris). [Being and Nothingness; cited for bad faith (mauvaise foi) as Level 2 obstacle class and for the ontological necessity of bounded recursive self-improvement in pour-soi consciousness.]

Saxe, R., and Kanwisher, N. (2003). People thinking about thinking people: The role of the temporo-parietal junction in "theory of mind." *NeuroImage*, 19(4), 1835-1842.

Simon, H. A. (1973). The structure of ill-structured problems. *Artificial Intelligence*, 4(3-4), 181-201.

Sutton, R. S., and Barto, A. G. (1998). *Reinforcement Learning: An Introduction*. MIT Press.

Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. *Cognitive Science*, 12(2), 257-285.

Varela, F. J., Thompson, E., and Rosch, E. (1991). *The Embodied Mind: Cognitive Science and Human Experience*. MIT Press.

Wiener, N. (1948). *Cybernetics: Or Control and Communication in the Animal and the Machine*. MIT Press.

Wollstonecraft, M. (1792). *A Vindication of the Rights of Woman*. J. Johnson (London). [Cited for sociological-structural constraint analysis as Level 3 obstacle class: barriers that individual-ring IP execution cannot remove.]

van Lamsweerde, A. (2001). Goal-oriented requirements engineering: A guided tour. *Proceedings of the 5th IEEE International Symposium on Requirements Engineering (RE'01)*, 249-263. [Cited for goal-traceability requirements in BDI/planning agent systems as C-B132 class analog.]

Wang, X., et al. (2021). Deconfounded recommendation for alleviating bias amplification. *Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery and Data Mining*, 1717-1725. [Cited for deconfounded recommendation as C-B132 class analog in recommendation systems.]

Yannakakis, G. N., and Togelius, J. (2011). Experience-driven procedural content generation. *IEEE Transactions on Affective Computing*, 2(3), 147-161. [Cited for experience-driven PCG / player preference learning as C-B132 class analog in game AI.]

Yudkowsky, E. (2008). Artificial intelligence as a positive and negative factor in global risk. In N. Bostrom and M. M. Cirkovic (Eds.), *Global Catastrophic Risks*. Oxford University Press.

---

## Acknowledgements

Framework developed by Josh Mason (Human Living Institute). This preprint was drafted with AI assistance (Claude, Anthropic); all framework claims derive from the author's canonical documentation and are the author's intellectual work. AI assistance is acknowledged per field conventions for AI-assisted writing.

*ORCID: [Josh to add before submission]*

---

## Appendix A: Claims Register Summary

The full claims register is available at the project repository (see CITATION.cff). Summary statistics as of v0.36 (5 Aug 2026):

- Total claims: 165 (C1-C145, plus alias claims)
- ADOPTED (confidence >= 0.70, formally incorporated): 82 (most recently added: C137 ADOPTED 0.82 Level 4 biological-somatic obstacle taxonomy; C43 promoted to ADOPTED 0.90 1 Aug 2026; C138 promoted to ADOPTED 0.83 fold-cadence architectural mechanism)
- CANDIDATE (supported, under review): 59 (most recently added: C145 CANDIDATE 0.80 Design Attractor Hypothesis, 1 Aug 2026; C143 CANDIDATE 0.84 Method Layer Above Orchestration Layer, 1 Aug 2026; C131 ADOPTED 0.78 / C132 ADOPTED 0.82 / C134 ADOPTED 0.80 Prioritise Signal Map, 3 Aug 2026)
- HYPOTHESIS (speculative): 20 (most recently updated: C141 demoted from CANDIDATE 31 Jul 2026 -- incidental-disgust causal pathway failed replication)
- ARCHIVED (superseded): 0
- HELD (internal review pending): 4

Mean confidence across ADOPTED claims: 0.79. Confidence range: 0.70-0.90.

**v0.20 fold (30 Jul 2026):** Three structural extensions applied to the canonical: (A) Three-Level Obstacle Taxonomy (Section 2.6; Freud 1915/1923, Sartre 1943, Wollstonecraft 1792) in the Prepare substep; (B) Collective Effervescence account (Section 6.5; Durkheim 1912) in the multi-agent Experience layer; (C) BRSI Bracket grounding the bounded recursive self-improvement mandate in three independent philosophical traditions (Descartes 1641, Freud 1915/1923, Sartre 1943). No new claims added; all three extensions ground existing canonical positions in established philosophical literature.

**v0.21 fold (1 Aug 2026):** Four canonical extensions: (A) Level 4 Biological-somatic obstacle taxonomy (Section 2.6; C137 ADOPTED 0.82; functional medicine and disability studies -- Wolfe 2010, Barkley 2015, McEwen 2004) -- extends the taxonomy with a fourth level for practitioners with chronic illness, neurological differences, or metabolic conditions; (B) C101 Structural Mandation note at A3.5 Resource -- a mandatory per-cycle resource-elicitation question (not role presence alone) closes P3 Resource to STRONG (N=9 controlled comparison); (C) C102 Self-Replication Criterion note at A3.5 Become-Capable -- naming redundancy as the primary criterion predicts STRONG (N=9); (D) D.5.x Self-Redundancy Criterion in Section 6.6 -- the positive LOS design prescription derived from C102. Five canonical stale notes corrected.

**v0.22-v0.30 folds (1 Aug 2026):** Nine further canonical extensions applied: nine zero-mention ADOPTED claims given canonical body text (v0.22); new Part D Section D.6 Competitive Landscape and Category Validation added (v0.23); C138 fold-cadence section D.7 inserted (v0.24); universality stratification into implicit versus deliberate IP tiers in A0 (v0.25); R2R sixth-community consilience added to D.7 (v0.26); IP trait non-redundancy note in A0 (v0.27); C59 scale-invariance note in A4 (v0.28); Acrab GXLIX 1 hardware-native orchestration layer in D.6 with C143 confidence updated from 0.81 to 0.83 (v0.29); Active Inference Communicate prediction FIBV-P2 in D.5 (v0.30). No new claims minted in v0.22-v0.30.

**v0.31 fold (1 Aug 2026):** Mechanism-independent Perceive Stage 1 clarification applied (NX-B31021-MYCOPLASMA-PERCEIVE-1). The universality stratification paragraph in A0 now explicitly distinguishes gradient sensing via membrane biophysics (mechanism-independent; example: Mycoplasma pneumoniae navigates chemical gradients without Che proteins or methyl-accepting chemotaxis proteins) from dedicated receptor-signalling cascades (mechanism-implemented, Stage 2+). This confirms that Perceive as a functional criterion is substrate-independent of its molecular implementation, reinforcing C93 substrate universality. No new claims minted.

**v0.32 fold (3 Aug 2026):** Educational psychology / spaced-repetition research added as seventh independent consilience community for C138 (fold-cadence architectural mechanism). Source: Cepeda et al. 2006 meta-analysis (254 studies, approximately 14,000 participants) -- optimal inter-study interval for episodic-to-semantic consolidation = 10-20% of target retention interval; Cepeda et al. 2008 refinement: 5-10% for longer retention intervals. Provides quantitative calibration for the cadence-proportionality principle. C138 confidence updated 0.82 to 0.83 (seven-community consilience). No new claims minted.

**v0.33 fold (3 Aug 2026):** Prioritise Signal Map folded into A2 Prioritise substep as a coordinated four-signal framework. Three signals grounded and newly ADOPTED: C131 positive-valence-at-Prioritise signal (low-arousal positive validates Define completion; Reber and Schwarz 2004, Emmons and Diener 1986, Gendlin 1978; ADOPTED 0.78); C132 anxiety-at-Prioritise contamination (anxiety at Prioritise signals Define contamination -- fear about the goal rather than genuine comparative ranking; ADOPTED 0.82); C134 BAS-CLASS contamination (strong approach motivation may bypass Define via Behavioural Activation System; ADOPTED 0.80). A fourth signal placeholder (C121 excitement, HELD) reserved pending ratification.

**v0.34 fold (3 Aug 2026):** Stage 1 substep ordering and three-level sub-structure added to A0 universality stratification paragraph. Two convergent biological evidence lines: (A) Partial-order boundary -- Perceive emerges first via membrane biophysics at minimal hardware cost; Prioritise and Plan require dedicated neural circuitry (Stage 2+). (B) Three-level Stage 1 sub-structure: (a) Mycoplasma class: implicit Perceive only, no Define analogue; (b) E. coli CheR/CheB class: implicit Perceive + implicit Define (methylation setpoint as homeostatic reference); (c) Dedicated Che cascade: mechanism-implemented Perceive + mechanism-implemented Define. Extends C90 causal-closure ordering to the mechanism-implementation level. No new claims minted.

**v0.35 fold (5 Aug 2026):** Stage 2a/2b/3 mechanistic sub-stratification added to A0 universality stratification paragraph. Stage 2a: ganglionic circuits (approximately 8-12 neurons; C. elegans AIY class) = proto-Simulate threshold. Stage 2b: mushroom-body circuits (approximately 2,000 Kenyon cells; Drosophila) = proto-Plan threshold. Stage 3: lateral habenula counterfactual signal onset (Matsumoto and Hikosaka 2007, 2009) = Stage 3 boundary. Grounds Stage 2 and Stage 3 transitions in specific identified neural circuit classes. No new claims minted.

**v0.36 fold (5 Aug 2026):** mem0 ADD-only engineering corroboration added within C138 D.7 community (2) entry. mem0 is the top-performing system in the 2026 "State of AI Agent Memory" benchmark at 91.6 LoCoMo accuracy; it uses pure accumulation with no consolidation governance -- independently confirming the accumulation-without-consolidation gap that C138 addresses. This is a 2026 production engineering convergence: the field's leading memory system exhibits the exact failure mode C138 prescribes against. No new claims minted.

The register is machine-readable (CSV/XLSX) and human-readable (Markdown index). Each claim file includes: claim ID, title, formal statement, confidence score, status, evidence basis, and cross-references to related claims.

---

## Appendix B: Void Taxonomy

MOEMOI's motivational architecture identifies five deficit void types and one generative drive, grounded in empirical research:

- **Epistemic void:** Gap in understanding/knowledge. Resolution: accurate Understand.
- **Conditional void:** Perceived condition (safety, security) not met. Resolution: Define the structural constraint; Prepare around it.
- **Competence void:** Gap between current and required capability. Corresponds to SDT competence need. Resolution: deliberate practice via the Do/Learn cycle.
- **Relational void:** Gap in connection, belonging, or recognition. Corresponds to SDT relatedness need. Resolution: Communicate substep primarily.
- **Autonomy void:** Gap in self-direction, perceived control, or agency. Corresponds to SDT autonomy need. Resolution: Define-authority must be preserved; any system that removes the practitioner's Define-authority converts the autonomy void into a structural constraint.
- **Generative drive:** Not a deficit, a forward-directed motivation toward creation, growth, or contribution that activates when deficit voids are adequately addressed. Motivational source for sustained high-IP% performance.

The taxonomy is grounded in SDT [Deci and Ryan 1985], information gap theory [Loewenstein 1994], and Maslow's hierarchy [Maslow 1943] (see C-void claims in the register for full provenance).

---

*MOEMOI v0.14 (v0.36 fold) | Preprint Draft v1 | 5 Aug 2026*
