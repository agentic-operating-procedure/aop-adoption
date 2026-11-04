# AOP Procedural Engineering Playbook (Adoption Scope)

Informative. This document states the six-stage playbook that moves one procedure from a classic SOP to a governed AOP. Each stage has an objective, activities, a gate, and evidence to keep. The gates are the point: a stage that has not passed its gate does not feed the next one. The worked demonstration of all six stages is the 5G anomaly management exemplar in `aop-examples`.

## Stage 1: Procedural decomposition

Objective: know what procedure you are actually migrating.

- Decompose the SOP estate into procedure families: which SOPs describe one operational procedure, which are variants of each other, which are stale.
- For the target procedure, state its intent, its outcome, and its scope boundary in the enterprise's own vocabulary. Associate it with the enterprise process catalog where a canonical entry exists, or declare the gap (CG-PA-1 to CG-PA-5).
- Keep: the decomposition map, the source SOP with its version, the process reference or gap.

Gate: the procedure family is named, the source SOP version is pinned, and the scope boundary is stated.

## Stage 2: Operational grounding

Objective: replace the SOP's claims with observations.

- Stand up the declared capture surface for the procedure family (CG-O1), under the observation posture.
- Stitch observed work into cases (CG-S1 to CG-S14). The SOP is a hypothesis: matches, variants, exceptions, workarounds and undocumented paths are classified against it.
- Publish the observed corpus with its provenance: stitching version, capture surface version, case counts.

Gate: the observed corpus covers the procedure family, the documented path's observed coverage is measured, and the undocumented paths are inventoried.

Evidence rule: if the documented path holds for a minority of cases, that is not a failure of the migration; it is the happy-path fallacy confirming itself, and it is the reason the migration is worth doing.

## Stage 3: Autonomy disposition

Objective: decide, per decision family, what the agent may do.

- Assess the procedure over the five risk axes (NM-AUT-5): risk, reversibility, operational impact, authority threshold, assurance requirement.
- Produce the governance manifest: permitted set, prohibited set, authority class per decision family with applies_to scoping where the family governs specific actions, the default authority class, skills and credentials.
- State the human baseline for the domain metrics (NM-ASR-2), bound each metric to the canonical catalog where one exists or declare the gap (NM-INT-5).

Gate: the manifest is complete, every permitted action is covered by the union of rules plus the default class, and no autonomous classification contradicts the risk-axis assessment.

Evidence rule: authority comes from the owner, never from the miner. Observation says what humans decided; this stage says what the agent may decide.

## Stage 4: AOP specification

Objective: compile and validate.

- Compile: SOP intent hypothesis plus observed corpus plus manifest, through the toolchain, into a versioned AOP with provenance (NM-PRV-1 to NM-PRV-3).
- Lint and conform: the document validates against the schema and passes profile AOP-DOC-1.
- Review the discrepancy between the SOP's claims and the compiled rules: every threshold the SOP stated in prose now carries its observed value, and the spread is visible.

Gate: the compiled AOP lints clean and the provenance chain verifies against the corpus.

## Stage 5: Harness engineering

Objective: run the AOP inside a governed boundary.

- Deploy or adopt the harness for the domain: the harness is itself specified as an AOP (SEC-11), with its boundary, credentials, escalation routes and verification obligations.
- Wire escalation: every approval-required route names a role and an evidence bundle; the approvers have seen a bundle before the first run.

Gate: the harness passes profile HAR-1; the harness's own AOP is conformant.

## Stage 6: Verification and assurance

Objective: earn the promotion, then keep it.

- Shadow mode: run the compiled AOP in observation-only mode against live cases; compare agent dispositions with human choices; review every discrepancy (P5.4). Promote to bounded execution against the declared promotion band, not against confidence.
- Bounded execution: every action appends to the case record; the baseline metrics are computed per week against the human baseline.
- Drift: the recalibration obligation (NM-CTL-4) is live; a drift observation produces a new AOP version through the governance process.

Gate: the shadow agreement is within the declared band and the first bounded runs carry complete case records. The live-value claim is made only from live bounded runs, published with the reproducibility protocol.

## The playbook in one line

Decompose, ground, dispose autonomy, compile, harness, verify. The SOP is the hypothesis; the corpus is the measurement; the manifest is the mandate; the AOP is the compiled standard; the harness is the boundary; the case record is the proof.
