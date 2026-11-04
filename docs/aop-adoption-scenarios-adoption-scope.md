# AOP Adoption Scenarios (Adoption Scope)

Informative. This document states the three adoption scenarios, their entry conditions, and their specific traps. The scenarios follow the deployment topologies in `aop-architecture`; this document is the adopter-side view of the same ground.

## Scenario 1: Pilot

A single procedure family, single harness, shadow first.

- Entry: one procedure family with a stable SOP, an observation surface it is permitted to declare, and a named approver role.
- Path: playbook stages 1 to 4 on the pilot family; shadow mode against live cases; bounded execution for the actions the risk axes justify; the rest stay approval-required.
- Trap: the pilot that proves nothing. A pilot on a procedure whose documented path already holds for nearly every case will show high agreement and teach nothing, because there was nothing to escape. Choose a family where exceptions are common; the happy-path fallacy is the business case.
- Exit: the shadow agreement within the declared band, bounded runs with complete case records, and the honest value statement: parity or improvement measured against the baseline, over a stated period.

## Scenario 2: Brownfield

An existing estate of SOPs, RPA and workflow engines gains a decision layer.

- Entry: significant existing automation; the SOP library is the human-readable source of truth.
- Path: deterministic steps stay with RPA and the engines; the AOP becomes the decision layer above them (ARC-T3): which variant applies, what the thresholds are, when to escalate. Observation extends to the legacy and UI-driven interactions the API view never shows, because that is where the undocumented paths live.
- Trap: retrofitting authority onto systems that cannot fail closed. Where the existing system cannot enforce a boundary, the AOP classifies its actions as approval-required at most and the harness holds the boundary itself.
- Exit: the decision layer governs the existing automation, and the observation corpus includes the legacy paths that were previously invisible.

## Scenario 3: Regulated and high-risk

The procedures where a wrong action has regulatory or safety consequences.

- Entry: a regulator, a licence condition, or a safety case governs the procedure.
- Path: everything in the pilot path, plus: the risk-axis assessment is reviewed by the compliance function; the authority-threshold axis is set conservatively; shadow mode runs until the agent's choices match human decisions at the observed rate for a stated period; the case record and its replay are demonstrated to the auditor; recertification is periodic and scheduled.
- Trap: the compliance review that arrives after promotion. In this scenario the conformance and evaluation evidence is prepared for the regulator's questions before the first bounded run, not after.
- Exit: bounded execution under the regulator's terms, with the evidence regime part of the licence condition's answer.

## Choosing

Most estates start with Scenario 1 on one family, grow to Scenario 2 as observation extends, and apply Scenario 3 to the families that need it. The scenarios differ in evidence and conservatism, not in the playbook: the six stages are the same, and the gates are the same.
