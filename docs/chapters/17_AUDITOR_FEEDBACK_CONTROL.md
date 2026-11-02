# Reward Controller: Adjusting Future Effort

A document-delivery application sends a reproduction and reports that the requested wording is available. Subsequent review finds that the relevant page was never checked. The delivery succeeded as a transmission, but its claim about the evidence was unsupported. Asking the application to “be more careful” leaves the next assignment almost unchanged.

The **Reward Controller** offers a more specific design: an auditor or outer loop evaluates the result and proposes bounded changes to future assignments. The change might add verification at the point where adequacy was previously assumed. It should follow the demonstrated difficulty and remain under the authority responsible for the application.

The repository specifies that feedback arrangement. It does not train model weights or provide an automatic learning service. Its useful idea is to connect an evaluation to an authorized adjustment while preserving a separation between producing work and deciding how that work should affect future effort.

## 1. Establish the result before evaluating it

Consider a trial with retained request, tool, and delivery records. A researcher asked about wording on a particular page. The application retrieved the reproduction and sent it, but its record contains no check of that page. A reviewer subsequently inspects the page and finds the passage unreadable in the supplied copy.

The example now has two kinds of material. The records and inspection establish events and findings. The auditor judges what those findings imply for task completion and the adequacy of the process.

| Evidence or judgment | What it establishes in this trial |
|---|---|
| Delivery record | The reproduction was sent. |
| Page inspection | The supplied copy does not make the requested passage readable. |
| Task judgment | This delivery did not meet the stated wording need. |
| Process judgment | A pre-dispatch adequacy check could have exposed the unsupported claim. |

*Decomposition* separates delivery, evidence adequacy, and task completion. *Comparison* relates the delivered result to the actual request. *Inference* identifies a plausible corrective step. Their combination prevents a successful transmission from standing in for successful research access.

The final judgment has a narrower status than the inspection. It proposes a process improvement; it does not establish that the next run will perform better. If the page had never been inspected, its readability would remain unknown even though the missing check was already evident.

## 2. Give the auditor authority over feedback

The controller's owner is the **auditor**. Its contract excludes ownership by the inner agent, primary solver, and branch generator. An inner agent may not optimize or rewrite its own reward target. The auditor or outer loop gates changes affecting future assignments.

The separation has a concrete consequence in the archive trial. The solver cannot count “file sent” as sufficient success merely because that description favors its result. The governing request supplies the evidence need; the auditor assesses the result against it. A solver's explanation can contribute material for review, while the request, records, and inspection remain available to challenge that explanation.

*Role abstraction* distinguishes producing a result from assessing its consequences. *Topological arrangement* puts the authorized review between evaluation and assignment change. *Evaluation* checks whether the proposed change remains within that authority. Together they keep feedback accountable to something beyond the solver's preferred account.

An application may assign review to a person, a separately instructed model, or another suitable process. Merely naming a second model “auditor” does not create independent evidence. It still needs the relevant records and criteria, and the host must decide which changes it may approve.

The source calls its outputs `auditor_reward_report` and `dial_nudges`. The report carries the evaluation; the nudges propose adjustments. Neither output independently grants permission to alter the application.

## 3. Translate a diagnosis into a particular adjustment

The controller names four targets in an external assignment system, PSPE: planning, exploration, verification rigour, and clarification frequency. These are future-assignment controls. The repository does not bundle the host that makes them operational.

A designer can begin with the effect each control is meant to have:

| Assignment dial | Possible application adjustment |
|---|---|
| Planning | Require the plan to identify which evidence must be obtained before delivery. |
| Exploration | Allow another evidence route when the first copy cannot serve the request. |
| Verification rigour | Require inspection of the relevant passage before claiming adequacy. |
| Clarification frequency | Seek clarification when the request leaves the needed feature unclear. |

The trial chiefly supports a verification adjustment. The request was already specific. Asking the researcher more questions would not replace the omitted inspection. Increasing exploration would also miss the immediate issue if the application continued selecting copies without checking them.

*Classification* locates the failure in the process. *Controlled variation* changes the assignment where that failure occurred. *Comparison* asks whether the change addresses the observed gap. Their combination makes feedback more selective than increasing every kind of effort after an unsuccessful result.

The next comparable assignment might therefore require a recorded adequacy check before dispatch, with deferral when the relevant passage cannot be read. That is a proposed interpretation of a verification nudge. The host needs to define how its dial maps to that instruction, what resources the check may use, and how compliance will be reviewed.

## 4. Keep bounds and priorities meaningful

The specification names truth, task completion, coherence, attunement, humility, safety, and divergence inputs. It includes weights, caps, cooldowns, a bounded update parameter, and a priority order beginning with safety and truth. Its anti-wireheading controls block positive reward when safety or truth is low and prevent the inner agent from updating its reward.

These controls express an intended relation between criteria. A useful delivery cannot compensate for an unauthorized disclosure, and fluent explanation cannot compensate for a false claim about readability. The application needs defined criteria and a gate that preserves those priorities.

The numerical settings remain design proposals. For example, `alpha: 0.02` names a bounded-update parameter; it does not define a calibrated two-percent improvement or a universal change in verification effort. The host must supply the update rule, dial scale, allowable range, and basis for judging an adjustment.

The same requirement applies to specialized inputs. A KL-divergence value needs defined distributions and a reference against which divergence is computed. A stylistic impression cannot supply that measurement. A deception penalty needs grounds for the relevant finding; an incorrect result alone does not establish deception.

*Decomposition* separates priority, evaluation, and update magnitude. *Concretization* specifies what an accepted nudge would change. *Evaluation* checks the change against governing limits. This combination allows feedback to be restrained without treating an unexplained number as an instrument.

## 5. Revisit the change through comparable outcomes

The update policy applies to **future assignments only** and requires an auditor or outer-loop gate. In the trial, the existing delivery still needs an appropriate correction. Changing a future verification instruction cannot retroactively make that delivery adequate.

For a later comparable request, the reviewer can examine whether the proposed check occurred, whether it exposed missing evidence, and whether the resulting delivery served the request. The check may also add delay or unnecessary work. A useful review retains those costs alongside any improvement. If the later task differs materially, its result needs that context before it informs another adjustment.

The controller's added capability is a bounded feedback path: observed result, grounded evaluation, targeted suggestion, authorized future change, and subsequent review. Each connection can be inspected. The source design leaves the application responsible for supplying outcome records, evaluators, operational dial meanings, and enforcement.

> Review the document-delivery trial using the request, execution records, delivered response, and page inspection. Separate actual findings from judgments about task and process quality. Identify the smallest future-assignment adjustment supported by the omitted adequacy check. State the proposed dial, its operational effect, and the auditor or outer-loop gate required to accept it. Preserve safety and truth priorities. Leave unsupported numerical or divergence inputs unavailable, and keep the solver from rewriting its success criterion. Specify what a later comparable outcome would need to show before retaining or revising the adjustment.

The shared appendix gives examples of how to carry such bounded requests and findings between stages. A structured handoff can preserve the grounds for a change; its structure does not establish that the change has been implemented or has improved an outcome.

Reference: [Reward Controller specification](../../framework/RewardController_ParallaxEngine.v1.json) · [Reward Controller guide](../../reference/skills/REWARD.md) · [probe profiles](../../reference/skills/PROBES.md) · [evaluation boundaries](../appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#3-distinguish-illustration-from-evidence) · [external companions](../../reference/PROVENANCE.md#external-companions).

[Previous: Organ Atlas: Observing the Application](16_OBSERVATION_AND_RECOVERY.md) · [Next: Open Questions and Further Directions](18_OPEN_QUESTIONS_AND_FURTHER_DIRECTIONS.md)
