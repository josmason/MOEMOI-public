# Contributing to MOEMOI

MOEMOI is an open, testable framework. Its usefulness depends on being tested against evidence, including evidence that parts of it are wrong. This file explains how to engage.

---

## What counts as a contribution

### Empirical challenges
The most valuable contributions are evidence that changes the confidence level of a specific claim.

Every claim in the register has a C-number, a status (Hypothesis / Candidate / Adopted), a confidence level, and a kill-line: a specific result that would force a downgrade. If you have:
- A study whose results conflict with a CANDIDATE or ADOPTED claim
- Data that strengthens a HYPOTHESIS toward CANDIDATE
- A replication that confirms or fails to confirm a claim

Raise it as a GitHub Issue with the relevant C-number in the title (e.g., "C21 — counter-evidence from ..."). Link the paper or dataset. State how the evidence changes the kill-line threshold.

### Structural critiques
If you think the IP loop is missing a necessary step, duplicating an existing one, or carving at the wrong joint, that is worth raising. State the argument in terms of what the framework predicts incorrectly as a result of the structural flaw, and what the alternative predicts better.

### Derivative frameworks
If you are building on MOEMOI — adapting it to a specific domain (organisations, clinical settings, AI evaluation, education) — open an Issue or link the derivative work. The claims register is designed to accumulate evidence from multiple applied contexts. Attribution under CC-BY 4.0 is all that is required.

### Terminology and vernacular
The framework uses a specific vocabulary (MOEMO, the IP, the void taxonomy, BRSI). If a term creates confusion or maps onto an established concept in a way that should be acknowledged, note it. The vernacular is not sacred; it is a tool.

---

## What is not in scope here

### Feature requests for CoLive
CoLive (the Life Operating System product built on MOEMOI) has its own development track. Feature requests, UX feedback, and implementation ideas belong in a separate CoLive repo when that is published. This repo is for the theoretical framework, not the product.

### Values disputes
The framework deliberately does not specify what you should want. The Define step — what gap to close, what to optimise toward — is explicitly left to the practitioner. If you disagree with someone's goals, that is not a claim about the framework. The framework is about how to close gaps, not which gaps to close.

### Requests to lower confidence on non-empirical grounds
Confidence levels in the register are evidence-determined. An argument that a claim "should" be less certain because it is ambitious or because the author is unknown is not evidence. Bring data or a structural argument.

---

## How the claims register works

Every claim has a file in `Registers/Claims/` with:
- The claim text
- The current evidence summary
- The confidence level with a narrative explanation of what raises or lowers it
- A kill-line: a specific empirical result that would force a downgrade
- A history of updates

When you raise an Issue that changes a claim's evidence status, the maintainer will update the per-claim file and regenerate the register index. The change will be visible in the commit history.

This is the mechanism that keeps the framework honest over time. It is also what distinguishes MOEMOI from a book of advice: books do not update when evidence changes.

---

## How to raise an Issue

Use this template:

```
Title: C[number] — [brief description of the evidence]

Type: [empirical challenge / structural critique / derivative / terminology]

The claim: [paste the current claim text from the register]

The evidence: [citation or argument]

Effect on confidence: [your assessment of how this changes the claim's status or level]

Kill-line status: [does this meet the kill-line? If not, how close?]
```

You do not need to know the answer. You can raise an Issue as a question: "The claim at C42 assumes X, but I found Y — does this change anything?" That is a valid contribution.

---

## Open research problems

The README lists five pre-specified open research problems (RP1 through RP5) that represent the highest-leverage open empirical questions in the framework:

- **RP1** — Does the completeness score predict outcomes? (pre-registered comparative test)
- **RP2** — Does the IP structure hold across substrates beyond human cognition?
- **RP3** — Can the claims-register methodology transfer to other frameworks?
- **RP4** — Does recursive self-improvement at the harness layer converge with 2026 AI architectures?
- **RP5** — Is the void taxonomy a valid diagnostic instrument?

If one of these matches your research area, that is the most direct route to a contribution that changes confidence levels in the register. The full problem statements, including the specific evidence that would move each claim, are in the README under "Open research problems."

---

## Pre-registered comparative tests

The framework makes a specific falsifiable prediction: a practitioner running the IP more completely (higher completeness score) will show better outcomes than a matched practitioner running it less completely. This is the most direct empirical test.

If you want to run a pre-registered test:
1. State your hypothesis and kill-line in a GitHub Issue before collecting data.
2. Specify the outcome measure, the completeness scoring method, and the sample.
3. Run the test and report the result, regardless of direction.
4. The maintainer will update the relevant claim's evidence summary and adjust the confidence level accordingly.

Pre-registration before data collection is the standard that makes the claims register defensible over time. Results that run the test but were not pre-registered are still welcome; they are logged as exploratory and weighted accordingly.

---

## Attribution and license

CC-BY 4.0. You are free to share, adapt, and build on this material for any purpose, including commercially, as long as you give appropriate attribution.

If you contribute evidence that changes a claim, you will be credited in the per-claim file's update history.

If you build a derivative framework, citing the relevant claims is sufficient attribution (see the README for citation formats).

---

## Contact

For questions that do not fit the Issue template (conceptual questions, collaboration proposals, derivative work you are building), open a GitHub Discussion or raise a GitHub Issue tagged "discussion."

For direct correspondence about the framework, email: joshmason@humanlivinginstitute.org

Response time is not guaranteed, but substantive empirical engagement is always welcome.

---

*MOEMOI is meant to spread, not to be owned. The ideas should move into the places where they are most useful, tested there, and returned to the register as evidence.*
