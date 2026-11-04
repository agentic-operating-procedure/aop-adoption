# AOP Adopter Checklists (Adoption Scope)

Informative. One checklist per playbook stage, written to be used without the programme stewards in the room. Each item is a gate condition; an unchecked item means the stage is not done.

## Stage 1: Procedural decomposition

- [ ] The procedure family is named, and the SOPs that describe it are listed with versions
- [ ] The intent and outcome are stated in one sentence each, in the enterprise's own vocabulary
- [ ] The scope boundary states what is in and out of scope
- [ ] The enterprise process catalog reference exists, or the gap is declared and lodged
- [ ] The source SOP version is pinned and stored

## Stage 2: Operational grounding

- [ ] The capture surface is declared, versioned, and privacy-reviewed (CG-O1)
- [ ] Cases are stitched with the domain correlation key, with stitching version recorded
- [ ] The documented path's observed coverage is computed and published
- [ ] Undocumented paths, workarounds and exceptions are inventoried
- [ ] Unstitchable events are quarantined with reasons, not deleted (CG-S10)

## Stage 3: Autonomy disposition

- [ ] The five risk axes are assessed and recorded per decision family
- [ ] The governance manifest states permitted, prohibited, authority per family with applies_to scoping, and the default class
- [ ] Every permitted action is covered by rules plus the default class
- [ ] No autonomous classification contradicts the risk axes
- [ ] The human baseline metrics are stated, each bound to the canonical metric or declared as a lodged gap (NM-INT-5)
- [ ] Every named approver knows they are named

## Stage 4: AOP specification

- [ ] The compiled AOP validates against the schema and passes profile AOP-DOC-1
- [ ] Every decision rule carries observed provenance
- [ ] The SOP's prose thresholds now carry their observed values, and the spread is reviewed
- [ ] The provenance chain verifies against the corpus
- [ ] The identifier and version follow the scheme; lifecycle status is on three dimensions

## Stage 5: Harness engineering

- [ ] The harness is itself specified as an AOP and is conformant (SEC-11)
- [ ] Profile HAR-1 passes on the harness
- [ ] Every approval-required route names a role and a complete evidence bundle
- [ ] Credentials are scoped per action class; high-risk classes require prior approval
- [ ] The escalation roster is staffed and the ruling-latency metric exists

## Stage 6: Verification and assurance

- [ ] Shadow mode ran against live cases; every discrepancy was reviewed
- [ ] The shadow agreement is within the declared promotion band
- [ ] The promotion decision is recorded in governance, not assumed
- [ ] Bounded runs append complete case records; the chain verifies
- [ ] The drift obligation is live: bands declared, recalibration routes to a new version
- [ ] Any value claim is published with the reproducibility protocol, against the baseline

## Estate-level (per period)

- [ ] The maturity stage is stated per procedure family, with evidence
- [ ] Regressions from suspensions are reflected in the maturity statement
- [ ] Recertification is scheduled for every conformant artefact whose digest changed
- [ ] The lodged metric and process gaps are tracked to closure in the catalogs
