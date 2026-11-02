# Applying and Assessing a Method

The chapters develop ways to represent a problem, transform its relationships and organize useful methods. This appendix brings the working references together: describe the case, try a transfer, and distinguish what an illustration shows from what an actual use establishes.

The examples below are original illustrations. The separately linked evaluation supplies recorded outputs for particular tasks. Keep the source, proposed operation and resulting evidence available when adapting either to another application.

## 1. Represent the case

O/D/R/O separates four related aspects of a description. It is a lexical structure, not an embedding format, and does not need a particular model to read it.

| Field | Meaning | Access-dependency example |
|---|---|---|
| Ontology | The entities, roles or relationship being described. | A competent practitioner and a separate controller of necessary access. |
| Dynamics | The process or relationship that produces or maintains a state. | Skill increases while access remains controlled elsewhere. |
| Regime | Conditions under which that description holds. | The controlled access is necessary and no viable alternative is available. |
| Outcome | A supported or conditional consequence. | Completing this task remains dependent on the access controller. |

### Outcome and destination

The final O is used as *outcome* in the evaluation and as *destination* in some memory and transformation contexts. A consumer must know which interpretation it is receiving.

- An **observed outcome** records evidence of what happened.
- A **predicted outcome** states what a hypothesis implies, with uncertainty.
- A **desired destination** states an authorized objective.

Keep these statuses explicit in the surrounding record. An intended result must not silently become an observed fact. The existing source packet formats are preserved; this documentation does not introduce a replacement schema.

### Boundaries of the representation

O/D/R/O helps organize claims; it does not verify them. Preserve a source pointer, mark unknowns, and distinguish an extracted relationship from a proposed analogy. Do not infer motives from a structural description. A similar shape in another domain suggests a candidate method, not proof that the same explanation applies.

## 2. Carry the relation into an application

### What should transfer?

A concept is reusable when its governing relationship and necessary conditions survive a change of setting. The technician's name and the workshop's location may be incidental. The necessity and control of access are consequential.

“Skill never produces independence” loses the condition. Merely repeating the technician's story leaves the abstraction implicit. A useful statement is narrower: competence alone does not remove a dependency created by externally controlled necessary access.

In this example, control of access belongs in the dynamics, and the exclusivity and necessity of access qualify the regime. Those choices can be inspected and challenged. Different tasks may support more than one useful representation.

### 1. Extract a relationship without making it universal

**Source:** A repair team can diagnose a failed pump. Another organization alone can unlock the control cabinet required to repair it. No alternative access route is currently available.

**Method:** KCE, with the O/D/R/O distinctions.

**Candidate concept:** Technical competence does not remove dependence on a party that exclusively controls necessary access.

**Check:** The source supports diagnosis, not mastery of every repair. It does not establish refusal or hostile intent. A viable alternative access route would change this particular dependency.

Try supplying the source and method to a model, then inspect whether its concept preserves those qualifications. Compare against the same task without the method; keep all attempts.

### 2. Preserve disagreement while enabling action

**Situation:** Two groups share a maintenance system. One wants more control over upgrades; the other wants dependable shared operating standards. Both still need the maintenance system.

**Method:** Coupler and CREM, with comparison if several proposals remain viable.

**Candidate reframe:** Distinguish authority over an upgrade from responsibility for shared operating standards. Consider an arrangement that separates those decisions while retaining the shared maintenance dependency.

**Check:** The proposed distinction is a candidate, not an agreement already reached. Neither group's demand establishes that its preferred arrangement is feasible. Practical cooperation need not imply trust or resolution of the underlying dispute.

### 3. Guide an article's movement

**Task:** Write an analysis of a fictional infrastructure negotiation using only supplied facts.

**Contextual guidance:** Establish the shared objective; distinguish technical feasibility from approval authority; preserve the parties' different dependencies; develop a conditional proposal only after the diagnosis.

**Check:** Does the finished article follow the relevant relationships without inventing a withdrawal, a motive or a successful negotiation? Does it read as an article rather than as a list of control instructions?

The [KCE evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) supplies a concrete version of this experiment, including the Kissinger framework and a rubric. Consult its task files for exact model inputs and its separate review materials for scoring.

### A compact trial instruction

> Use the supplied facts as evidence. Identify the governing relationship and the conditions under which it applies. Apply only the cognitive method relevant to the task. Give the requested answer, followed by a short record of the method used, preserved constraints and unresolved uncertainty. Do not invent numerical measurements or imply that a proposed check has been performed.

This instruction is a starting point. The source specifications offer fuller stage and handoff definitions when a task requires them.

## 3. Distinguish illustration from evidence

The framework is an explicit method collection. Its documentation, implementation in another project, successful use on one task and general effectiveness are different kinds of evidence.

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) includes:

- Encoding exercises: passage to governing concept, O/D/R/O and limits.
- A decoding exercise: a supplied Kissinger analytical framework and fictional facts to a new article.
- Separate dimensions for overgeneralization, undergeneralization, fidelity, structural transfer, writing quality and control-material leakage.
- An example report comparing Sol 6.1 at low reasoning effort with Qwen 3.8 27B, Q4_K_M, with thinking disabled.

The article task receives a prepared framework; it does not consume the model's preceding extraction. The example report contains six encoding cases and one article case per model, with separate, identity-masked AI review. Its judgments are provisional and have not been human-calibrated. Different backends and settings are recorded. This is evidence about particular outputs, not a broad model ranking or validation of every framework module.

## 4. Assess a new use

Use comparable task inputs and settings across ordinary instructions and structured-framework conditions. Define the scoring criteria before examining outputs. Keep all attempts, failures and uncertainty; use reviewers who do not know the tested condition where practical. Evaluate new cases, including cases where the method should be suppressed.

Check whether any improvement is due to the framework's structure, the additional task information or simply a larger context budget. Measure costs as well as output quality. Repeated trials and independent human review matter before making general claims.

## 5. Instrumentation boundaries

The JSON source specifications contain conceptual scores, thresholds, telemetry fields and runtime-probe proposals. This documentation release does not supply the instruments required to measure latent instability, neural attention, divergence, reward or every named confidence signal. A model-generated number is not automatically such a measurement.

Likewise, a schema-valid packet establishes only a structural property. Its source claims, applicability and proposed actions still require independent checks. Do not convert agreement between model roles into independent evidence of truth.

[Previous: Structured Handoffs and Packet Examples](A_STRUCTURED_HANDOFFS.md) · [Book contents](../../README.md) · [Technical reference index](../../reference/MODULES.md)
