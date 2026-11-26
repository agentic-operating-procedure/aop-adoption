# AOP Assessment Model (Capability Scope)

Informative. This document states the maturity path from human-operated to autonomous operations, and the obligations that attach at each stage. The model exists so an organisation can state honestly where it is, and so the word "autonomous" is never used as an aspiration when it is actually an earned stage with obligations.

## The four stages

| Stage | Name | What holds | Governing obligation |
|---|---|---|---|
| 1 | Human-operated | People execute the procedure from documents. The corridor works because a human notices what the document missed. | None of this programme's; the observation posture applies from the moment capture begins |
| 2 | Assisted | Agents propose; humans decide and execute. Every proposal is a draft, every decision is a person's. | Proposals carry their evidence; the human sees what the agent saw |
| 3 | Agentic | Agents execute bounded actions inside the harness under AOP authority; humans hold exception ownership. Approvals arrive as evidence bundles. | The full model: guardrail outside the context, scoped credentials, append-only records, conformance of the harness |
| 4 | Autonomous | Agents execute, measure and improve governed operations alongside people at the declared scope. "Autonomous" describes the degree of independent execution, not the absence of people. | Everything at stage 3, plus: drift response live, recertification periodic, the value claim measured against the baseline under the reproducibility protocol |

Stage 2 to 3 is the industry's typical frontier, and it is the transition this programme engineers for. Stage 4 is earned by evidence, not announced by policy.

## What does not change across the stages

- Accountability is human at every stage. The approver of record for a decision class is a role held by people; an agent is never the accountability sink (AOP-P07 in the discipline's principle set).
- The evidence obligation grows as autonomy grows: a stage 4 organisation has more evidence per case, not less, because more of the work is machine-executed and therefore needs machine-complete records.
- The corridor does not return. Once decision rights are explicit per decision, "the human notices what the document missed" stops being a safety mechanism and becomes an exception-handling discipline with its own routes and thresholds.

## The stage migration rule

AD-M1: An organisation MAY claim stage n when it satisfies the obligations of stage n across the procedures in scope, evidenced by case records, and not merely on a pilot. A pilot at stage 3 is a stage 2 estate with an exception, and stating it that way is the honest form.

AD-M2: Regression is allowed and reported. A drift event that suspends an AOP moves the affected procedures back a stage until the new version is effective; the maturity statement reflects it.
