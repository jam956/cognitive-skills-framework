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

## 6. Source and version notes

### Publication source

The `framework/` directory contains 23 JSON definitions and templates and one agent-facing skill guide from the `skills/cognitive-tools` package in `bounded-route-hyperagent`, source commit `dc6b7e536aeace455637fa22ce08edbbade712c4`. All 23 JSON files remain byte-preserved. The [manifest](../../SOURCE_MANIFEST.json) records the current files and their size and SHA-256 identities.

The original publication also included three usage guides and a historical CREM PDF under `framework/references/`. Their important content is now incorporated into the chapters and Appendix A. The manifest retains their former identities and links to the preceding publication for source inspection. The separate quick guides and file index have likewise been consolidated into the book.

### Skill guide publication repair

The source guide's unquoted YAML description contained `design: the model`, which a YAML reader treated as a mapping delimiter. A folded scalar repairs that header while preserving the description wording. A subsequent navigation revision replaces its removed reference-directory pointers with Chapter 15 and Appendix A. All other instruction text is retained.

The manifest distinguishes these publication repairs from the upstream source revision and records the file identities before and after each change. The JSON contracts are unchanged.

### Reading the source specifications

- KCE's source module is named **Key Concept Extraction**; the evaluation uses **Key Concept Elevation** for the abstraction task. This publication retains both usages with their contexts.
- The Dynamical Prism's filename includes `v1.2`, while its internal reduced-core version is `v0.2.0_reduced_core`. Use the declared internal version when interpreting the model; the filename is retained for compatibility.
- Terms such as `design_stable_executable_spec` are historical design-status labels. They do not mean this repository includes an executable implementation or a validated cognitive instrument.
- Some source prose describes an answer as becoming “inevitable.” Read that as a design aspiration toward constrained, defensible selection, not a guarantee or a reason to discard uncertainty.
- Historical CREM prose describes an earlier development stage. Use the v1.3 JSON and Chapter 12 for the current split of ontology, dynamics and regime.
- Retired filenames are listed for migration context. They are not missing current components.

### PSPP's numerical policy

The [PSPP v5.0-lite artifact](../../framework/PSPP_v5.0_CandidateSystemComparator.json) is preserved as published. Its comparison method is clear, while two policy details need a consistent interpretation in an implementation:

- `lite_contract.dare_audit_surface` requires DARE review at pruning loss `>= 0.35` or fragility `>= 0.45`. The corresponding `operational_thresholds` are `0.45` and `0.55`. The file does not state a precedence rule or distinguish the two sets as separate stages.
- The minimal example reports a top-branch score margin of `0.05` and sets DARE audit to `recommended: false`, although the lite contract requires review below `0.08`. The example merges contributions for the Arbiter but does not explain an exemption from that trigger.

These are unresolved details within the source design. The chapter illustrates comparison and conditional selection without treating those numerical controls as calibrated measurements.

### External companions

The specifications mention related components such as MPE, PSPE, ECE, an arbiter, memory curators, runtime monitors and provider-specific instrumentation. These are external interfaces or historical companion designs. Their mention does not imply that an implementation is bundled or that it runs when the documents are read.

### Updating this publication

Keep explanatory edits distinct from source changes. A source refresh should identify its revision, update file hashes and record compatibility changes. Prospective arrangements in [Chapter 18](../chapters/18_OPEN_QUESTIONS_AND_FURTHER_DIRECTIONS.md) retain their open contract and implementation status. Development history and editorial records remain in the archive outside the main reading route.

[Previous: Structured Handoffs and Packet Examples](A_STRUCTURED_HANDOFFS.md) · [Book contents](../../README.md) · [Module and file index](A_STRUCTURED_HANDOFFS.md#module-and-file-index)
