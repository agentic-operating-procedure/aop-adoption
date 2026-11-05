# AOP Operating Modes and Promotion Gates (Adoption Scope)

Normative within the adoption tier. This document is CR-019: the risk-tiered operating model that connects the playbook's stages to a progressive rollout, with measurable promotion, demotion and stop criteria. It does not introduce a parallel maturity model; it aligns with the maturity model's stages and the architecture's deployment topologies, and it consumes the evaluation tier's protocol as its evidence source.

## 1. The five operating modes

Modes attach per action class, not per AOP: one procedure can run its diagnostics in `bounded` while its dispatches sit in `approval-gated`. The mode determines what the executor may do with the class, what evidence accrues, and what promotion requires.

| # | Mode | What the executor may do | Required controls | Evidence accrued |
|---|---|---|---|---|
| 1 | Observe-only | Nothing. The procedure is compiled and linted; the runtime never acts | Capture surface declared; cohort separation live | The shadow corpus and its provenance |
| 2 | Recommend | Propose dispositions for humans to execute; no side effects | Proposals carry evidence; a human decides and executes everything | Proposal quality against human outcomes |
| 3 | Approval-gated | Execute only after an per-action human approval (RA-15 bindings live) | Full approval object; oversight metrics; canaries | Approval latency, precision, override rate |
| 4 | Bounded | Execute autonomous-class actions inside budgets and scope caps; approval-class actions still gated | Budgets (NM-CRD-4), parameter schemas (RA-20), workload identity (SEC-16) | Full case records vs the human baseline |
| 5 | Expanded | Bounded plus enlarged budgets and envelope, per the promotion record | Everything in bounded, plus drift obligations live and recertification scheduled | Drift response time, exception trends |

AD-M1: The authority classes in the AOP's Authority dimension cap the modes: no mode lets an executor act more permissively than the ratified rules allow. Modes govern *which* permitted actions run without a human in the loop and under how much aggregate budget; they never widen authority.

AD-M2: Model confidence is never a proxy for authority: a mode transition is a governance decision taken on evidence (EV-P8), never on a score the executor reports about itself.

## 2. Promotion gates

AD-P1: Promotion from mode n to mode n+1 requires, at minimum:

- The pre-registered independent evaluation gates pass on held-out and prospective cohorts (EV-P4, EV-P8); elapsed time and happy-path streaks are never sufficient.
- The conformance tier for the artefact and harness is current at the digest (the certification process).
- No open authority violation from the shadow period; conservative deviations reviewed and dispositioned.
- The residual risks are enumerated and a named role has accepted them (EV-P8).

AD-P2: The promotion record is the evaluation tier's promotion record plus the governance decision; it names the AOP version, harness version, component matrix (NM-VER-8), population, envelope, cohorts, results with uncertainty, and the risk acceptor.

## 3. Demotion and stops

AD-D1: Demotion criteria are declared with the promotion criteria and are measurable: an authority violation in bounded mode, an oversight alert sustained past the declared window (failing-approver), a drift observation that crosses the recalibration band without a candidate version, or a budget breach pattern, each triggers demotion to the declared fallback mode.

AD-D2: The emergency stop (SEC-15) and per-scope revocation (NM-VER-6) override every mode instantly. A demotion is a change in operating mode; a stop is an enforcement action; both are recorded.

## 4. Conformance versus operational authorisation

AD-S1: A conformant AOP is not an authorised one. Conformance (the certification tier) says the document satisfies the model and the harness enforces it. Operational authorisation for a mode is a governance decision taken on the promotion record. Templates and registries distinguish the two claims explicitly: an artefact may be certified and unauthorised; it may never be authorised and uncertified.

## 5. Mapping to the maturity model

AD-M3: The modes are the mechanism under the maturity model's stages: stage 2 (assisted) is modes 1 to 2; stage 3 (agentic) is modes 3 to 4; stage 4 (autonomous) is mode 5 at scale. The maturity statement per procedure family cites the modes its action classes operate in. The scenario paths (pilot, brownfield, regulated) choose their entry mode by risk: regulated and high-risk families enter at mode 1 regardless of ambition.

## 6. What this document does not fix

The thresholds inside a promotion gate are pre-registered per procedure family (EV-P4); this document fixes the gate structure, not the numbers. Low-risk examples and a high-impact example with explicit residual-risk treatment are the exemplar programme's (CR-006) Wave 6 deliverables.
