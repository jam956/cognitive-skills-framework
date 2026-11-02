# Reference

This section gathers the source-file index, structured handoffs, application examples, evidence and source notes in one place. Use the entry that addresses the present question.

| What do you need? | Start here |
|---|---|
| Locate a definition or packet template. | [Source files and templates](#1-source-files-and-templates). |
| Prepare or interpret a handoff. | [Structured handoffs](#2-structured-handoffs). |
| Represent a case and carry its relation into another application. | [Applying a method](#3-applying-a-method). |
| Assess what an actual use establishes. | [Evidence and evaluation](#4-evidence-and-evaluation). |
| Inspect source versions, publication repairs or compatibility limits. | [Source and version notes](#5-source-and-version-notes). |

The handoff examples continue the archive's access-and-preservation case developed in [Chapters 9–15](../chapters/09_THE_CIRCLE_AND_THE_TILT.md).

## 1. Source files and templates

The seven separate templates have different jobs:

| Template | What the receiver needs to recover |
|---|---|
| [KCE v2.3](../../framework/KCE_Parallax_v2.3_PacketTemplate.json) | The working anchor, alternatives and information its compression might lose. |
| [Dynamical Prism v0.2](../../framework/Dynamical_Prism_v0.2_PacketTemplate.json) | The proposed operators and the conditions supporting their interpretation. |
| [Regime Field v0.1](../../framework/Regime_Field_v0.1_PacketTemplate.json) | Material constraints, uncertainty, permitted actions and reopening conditions. |
| [Prism Coupler v1.5](../../framework/Prism_Coupler_v1.5_PacketTemplate.json) | Which actors, roles, actions and conditions belong together. |
| [CTR v2.1](../../framework/CTR_Parallax_v2.1_PacketTemplate.json) | A selected movement, what it preserves and how its result returns to the question. |
| [ETE v1.1](../../framework/ETE_v1.1_PacketTemplate.json) | Distinct candidate systems, their checks and rejected or conditional routes. |
| [CREM v1.3](../../framework/CREM_v1.3_PacketTemplate.json) | Party distinctions, relationship dependencies and the proposed rebase. |

These records support different receiving questions. A simple access request may need only a small part of one record. A dispute about evidence, authority and resources may require several products to remain associated.

*Classification* selects the record appropriate to the unresolved issue. *Abstraction* retains its consequential content. Their combination reduces the amount carried while preserving what would change the next decision.

### Module and file index

The table connects each definition to the chapter that explains its purpose. Choose the needed contribution from the task, then inspect its source contract. The [packet index](../../framework/CognitiveTools_PacketTemplateIndex_v1.json) lists the optional full templates; load the selected template when its richer local structure is required. A module with an output schema inside its main JSON does not need a separate template.

| Component | Internal version | Role | Source | Book route |
|---|---|---|---|---|
| KCE | `v2.3.0` | Identify provisional anchors and compression risks. | [Specification](../../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) | [8](../chapters/08_KEY_CONCEPT_EXTRACTION.md) |
| CDP | `v1.2.0` | Select relevant domains and expose collision or lock-in risks. | [Specification](../../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) | [4](../chapters/04_ONTOLOGICAL_PRISM.md) |
| Regime profile | `v1.0.0` | Pass a compact constraint surface between stages. | [Specification](../../framework/CognitiveTools_RegimeProfile_v1.json) | [6](../chapters/06_REGIME_FIELD.md) |
| Dynamical Prism | `v0.2.0_reduced_core` | Describe primitive processes separately from conditions. | [Specification](../../framework/Dynamical_Prism_v1.2_ReducedCore.json) | [5](../chapters/05_DYNAMICAL_PRISM.md) |
| Regime Field | `v0.1.0` | Describe constraints, operating conditions and phase. | [Specification](../../framework/Regime_Field_v0.1.json) | [6](../chapters/06_REGIME_FIELD.md) |
| Coupler | `v1.5.0` | Bind ontology, actors, processes and regime. | [Specification](../../framework/Prism_Coupler_v1.5_OntologyDynamicsRegime.json) | [7](../chapters/07_PRISM_COUPLER.md) |
| CTR | `v2.1.0` | Select transformations and preservation checks. | [Specification](../../framework/CTR_Parallax_v2.1_SplitTransformRegistry.json) | [2](../chapters/02_WORKING_WITH_TRANSFORMATIONS.md#reference-examples-and-registry) |
| ETE | `v1.1.0` | Explore selected transformations and retain candidate branches. | [Specification](../../framework/ETE_v1.1_SplitLayerExplorationTransform.json) | [10](../chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) |
| CREM | `v1.3.0` | Rebase conflict and alignment while preserving dependencies. | [Specification](../../framework/CREM_v1.3_SplitOntologyDynamicsRegime.json) | [12](../chapters/12_RELATIONSHIP_REBASE.md) |
| PSPP | `v5.0.0-lite` | Compare and select, merge or defer candidates. | [Specification](../../framework/PSPP_v5.0_CandidateSystemComparator.json) | [11](../chapters/11_PARALLEL_SYSTEM_COMPARISON.md) |
| CEC | `v1.1.0` | Validate consequential ordering and dependency gaps. | [Specification](../../framework/CEC_Parallax_v1.1_ConditionalPathValidator.json) | [13](../chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) |
| DARE/IDCM | `v1.0.0` | Audit closure, pruning, missing operators and fragility. | [Specification](../../framework/DARE_IDCM_v1.0_ParallelSupervisoryLayer.json) | [14](../chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) |
| Probe profiles | `v1.0.0` | Choose a small sufficient route before loading full definitions. | [Specification](../../framework/CognitiveTools_ProbeProfiles_v1.json) | [15](../chapters/15_SELECTIVE_TOOL_ROUTING.md) |
| Organ Atlas | `0.3 (atlas)` | Describe optional monitoring and fail-safe probes; instruments are external. | [Specification](../../framework/Organ_Atlas_Template_v0.3.json) | [16](../chapters/16_OBSERVATION_AND_RECOVERY.md) |
| Reward Controller | `1.0` | Specify auditor-owned future feedback, not autonomous reward optimization. | [Specification](../../framework/RewardController_ParallaxEngine.v1.json) | [17](../chapters/17_AUDITOR_FEEDBACK_CONTROL.md) |

## 2. Structured handoffs

A comparison has selected a reproduction for one research request and left another request unresolved. The next component needs enough of that decision to answer correctly. “Use copies” loses the request, the adequacy check and the remaining need for original examination. Carrying every exploratory note would make the useful distinction harder to recover.

A handoff preserves the relationships the next act depends on. The packet templates provide places to record them. Their value appears when a receiving component can continue the work without inventing a missing condition or repeating the whole inquiry.

### Decide what the receiver needs

For the archive, a useful handoff identifies the request, the feature it requires, the proposed carrier, the result of any actual check, and what remains unknown. A binding question must not inherit a decision made for wording simply because both concern the same notebook.

*Decomposition* separates the request from its carrier and conditions. *Relation extraction* keeps their dependencies explicit. *Scope preservation* attaches a finding to the case it supports. Together they make a compact record possible without reducing it to an unsupported conclusion.

The [packet index](../../framework/CognitiveTools_PacketTemplateIndex_v1.json) names a thin common vocabulary, including `anchor`, `regime_profile`, `dynamical_profile`, `coupling_packet`, `transform_plan`, `branch_set` and `return_path`. A richer module record can preserve additional detail when it matters. The index's default is to load the relevant template selectively.

The examples below are **selected-field excerpts** from an illustrative archive case. Each block is valid JSON and uses the corresponding source record's field names. It omits parts of the full contract; it is not a complete execution result or a conformance fixture. Where a template leaves an array's item shape open, the example supplies small application records. The identifiers `A1`, `R1`, `B_copy` and `RP1` are local example references.

Unknown inspection results remain unknown. Numerical defaults in the templates are not filled merely to make an excerpt look complete.

### Follow one case through the template fields

#### KCE: retain the governing relationship

The anchor identifies what has to survive when “notebook access” becomes several possible routes. The provisional status keeps a later evidence problem able to reopen the framing.

```json
{
  "schema_version": "kce.parallax/2.3",
  "structural_statement": "A research request needs an evidence carrier that preserves the feature it asks about.",
  "anchor_candidates": [
    {
      "anchor_id": "A1",
      "anchor_statement": "Match each request to adequate evidence while retaining preservation conditions.",
      "anchor_type": "structural",
      "lock_status": "provisional"
    }
  ],
  "selected_working_anchor": {
    "anchor_id": "A1",
    "selection_reason": "Retains both evidence adequacy and preservation.",
    "lock_status": "provisional",
    "lock_allowed": false
  }
}
```

A receiver resolves `selected_working_anchor.anchor_id` against the candidate records. Carrying the identifier alone would not recover the anchor's meaning.

#### Dynamical Prism: preserve what is being done

Interpreting a request, checking a carrier and gating original handling perform different work. The excerpt names relevant clusters and their operators without inventing numerical strengths.

```json
{
  "schema_version": "dynamical_prism/0.2",
  "dynamical_profile": {
    "active_operator_clusters": [
      "information_representation",
      "boundary_control"
    ]
  },
  "active_operator_clusters": {
    "information_representation": [
      "detect",
      "interpret"
    ],
    "boundary_control": [
      "gate",
      "constrain"
    ]
  },
  "regime_field": {
    "resource_condition": "Supervision availability is unknown.",
    "uncertainty": "Copy adequacy is uninspected.",
    "legitimacy": "Original handling depends on actual authorization."
  }
}
```

The full template also has operator vectors, computed labels and mismatch reports. An application requiring those products supplies their grounds and interpretation. This excerpt leaves their numerical fields outside its scope.

#### Regime Field: keep missing conditions visible

The access route operates under conditions. A blank inspection result cannot become adequate evidence simply because a later stage expects a choice.

```json
{
  "schema_version": "regime_profile/0.1",
  "regime_profile": {
    "regime_id": "R1",
    "selected_working_regime": "Request-specific archive access",
    "regime_class": "other",
    "context_scope": "institutional",
    "active_constraints": [
      "The carrier must preserve the feature needed by the request.",
      "Original handling requires an authorized route."
    ],
    "evidence": [],
    "state_flags": [
      "copy adequacy unknown",
      "supervision unknown"
    ],
    "regime_shift_triggers": [
      "Adequate reproduction established.",
      "An original-handling route is authorized."
    ]
  }
}
```

The empty evidence array records that this illustrative excerpt supplies no completed inspection. The state flags preserve the specific questions still open. The shift triggers identify findings that could justify reconsideration.

#### Coupler: connect responsibility to a permitted action

The researcher states the evidence need; the archive's custodian establishes what can be supplied and handled. Separating actors and roles makes that responsibility inspectable.

```json
{
  "schema_version": "coupler.parallax/1.5",
  "source_refs": {
    "kce_anchor_ref": "A1",
    "regime_field_ref": "R1"
  },
  "coupling_packet": {
    "entry_mode": "relationship_binding",
    "actors": [
      {
        "actor_id": "researcher",
        "role_id": "requester"
      },
      {
        "actor_id": "archive",
        "role_id": "evidence_custodian"
      }
    ],
    "roles": [
      {
        "role_id": "requester",
        "description": "Identifies the feature to be studied."
      },
      {
        "role_id": "evidence_custodian",
        "description": "Confirms the available carrier and permitted handling route."
      }
    ],
    "qualifier": "reflective",
    "regime": "Request-specific archive access",
    "regime_ref": "R1",
    "permissioned_dynamics": [
      "interpret the request",
      "assess evidence adequacy"
    ],
    "suppressed_dynamics": [
      "treat unknown original-handling permission as granted"
    ]
  }
}
```

The small actor and role records are application-defined examples inside the template's open arrays. A deployment can use its own addressable identities. The essential connection is that an original-handling action remains attached to the authority and conditions that permit it.

#### CTR: retain the purpose of the movement

The distinction between evidence need and original handling creates another way to express access. The registry's actual dimensional-lift identifier keeps the selected movement traceable to its definition.

```json
{
  "schema_version": "ctr.parallax/2.1",
  "source_refs": {
    "anchor_ref": "A1",
    "regime_field_ref": "R1"
  },
  "transform_plan": {
    "selected_families": [
      "dimensional_family"
    ],
    "selected_operators": [
      {
        "operator_id": "CTR_DIM_LIFT_001",
        "label": "dimensional_lift",
        "family": "dimensional_family",
        "layer_targets": [
          "ontology_layer",
          "regime_field_layer"
        ],
        "preserves": [
          "conflicting_observations"
        ],
        "disturbs": [
          "dimensional_basis"
        ],
        "invoke_reason": "Separate the evidence need from original handling.",
        "requires_return_path": true,
        "verification_requirements": [
          "Check whether the proposed carrier preserves the needed feature."
        ]
      }
    ],
    "execution_order": [
      "CTR_DIM_LIFT_001"
    ],
    "return_path_requirements": [
      "Retain meaningful study and future preservation."
    ]
  }
}
```

Selection is the product shown here. ETE would develop what the movement permits; a carrier's adequacy still needs a suitable check.

#### ETE: make the alternative conditional in a useful way

The copy route becomes a branch with a return path and a distinguishing check. Its limitation for a binding request stays attached to the proposal.

```json
{
  "schema_version": "ete.parallax/1.1",
  "source_refs": {
    "kce_ref": "A1",
    "regime_field_ref": "R1"
  },
  "candidate_system_branches": [
    {
      "branch_id": "B_copy",
      "branch_type": "regime_projection_branch",
      "anchor_ref_or_shift": "A1",
      "regime_field": {
        "resource_condition": "A suitable reproduction may be available.",
        "uncertainty": "Its adequacy has not been inspected."
      },
      "return_path": "Serve the wording request using evidence that preserves the required feature.",
      "verification_requirements": [
        "Inspect the relevant passage and marks in the copy."
      ],
      "risk_notes": [
        "The binding request remains unresolved."
      ]
    }
  ],
  "rejected_branch_artifacts": []
}
```

The excerpt follows the source's `candidate_branch_schema`. Fuller branches also retain ontology, dynamics, coupling changes and scoring grounds where needed. An empty rejected-artifact list here does not establish that an exhaustive search found no other route.

#### CREM: preserve the parties while proposing a changed relationship

Researchers and conservators retain different responsibilities. A possible division of access routes can preserve those distinctions while leaving agreement unresolved.

```json
{
  "schema_version": "crem.parallax/1.3",
  "selected_mode": "productive_tension_preservation",
  "party_graph": {
    "party_nodes": [
      {
        "party_id": "researchers",
        "party_label": "Researchers",
        "protected_invariant": "The required evidence remains available for meaningful study."
      },
      {
        "party_id": "conservators",
        "party_label": "Conservators",
        "protected_invariant": "Present access preserves the collection's future usefulness."
      }
    ]
  },
  "dependency_invariants": [
    "A useful access route must preserve the evidence the request needs.",
    "Original-dependent study retains its handling and authority conditions."
  ],
  "relationship_rebase_plan": {
    "plan_id": "RP1",
    "mode": "productive_tension_preservation",
    "steps": [
      "Separate textual and material requests before choosing an access route."
    ],
    "preserved_dependencies": [
      "Evidence adequacy and preservation remain conditions on the proposal."
    ],
    "risks": [
      "Acceptance and original-handling permission are not established."
    ]
  }
}
```

A proposed plan is carried as a plan. Evidence for the source's validation gates and any actual acceptance would be separate work. The excerpt does not populate `validated_rebase_invariant` with an invented success.

Across these records, the additional capability is continuity of meaning: the original concern survives each local operation, and the next receiver can locate the remaining dependency.

### Translate into the receiving vocabulary

A source record and a receiving contract may organize the same contribution differently. The packet index supplies the common receiving names:

| Module product | Receiving field | Necessary translation |
|---|---|---|
| KCE's selected anchor reference and matching candidate | `anchor` | Resolve the selected identifier to the candidate's statement and conditions. |
| Dynamical Prism's profile | `dynamical_profile` | Retain the operator account and its interpretation. |
| Regime Field's compact profile | `regime_profile` | Carry material conditions and uncertainty. |
| Coupler's binding | `coupling_packet` | Preserve actor-role-action-condition associations. |
| CTR's selected movements | `transform_plan` | Preserve execution, return and verification requirements. |
| ETE's `candidate_system_branches` | `branch_set` | Keep branch identity, differences and limitations. |
| CREM's relationship account | `crem_packet` | Keep the party graph, dependencies, proposed rebase and gate status together. |

*Mapping* relates source products to receiver needs. *Identity preservation* keeps references attached to the records they identify. *Evaluation* checks whether a necessary qualifier survived translation. Together they make normalization an accountable operation.

There is a small source-vocabulary difference worth making explicit: the packet index uses `route_choice`, while the prose-first [skill guide](../../framework/SKILL.md#canonical-packet-contract) illustrates `route_used`. A receiving adapter chooses and documents its vocabulary, then maps that alias. Renaming it silently would leave two components appearing to agree while reading different fields.

Several modules define their products inside the main specification rather than in separate template files:

| Specification | Product to preserve |
|---|---|
| [PSPP](../../framework/PSPP_v5.0_CandidateSystemComparator.json) | Selected-system packet and decision artifacts, including remaining checks and selection grounds. |
| [CEC](../../framework/CEC_Parallax_v1.1_ConditionalPathValidator.json) | Path packet, dependencies and gap report. |
| [DARE/IDCM](../../framework/DARE_IDCM_v1.0_ParallelSupervisoryLayer.json) | Audit findings, rescued candidates, correction requests and reconstitution status. |
| [Probe Profiles](../../framework/CognitiveTools_ProbeProfiles_v1.json) | Routing decision, minimal output, suppression grounds and reopening trigger. |
| [Organ Atlas](../../framework/Organ_Atlas_Template_v0.3.json) | Qualified watch and recovery information when actual probes are supplied. |
| [Reward Controller](../../framework/RewardController_ParallaxEngine.v1.json) | Auditor report and bounded suggestions for future assignment dials. |

The compact [Regime Profile](../../framework/CognitiveTools_RegimeProfile_v1.json) and [CDP](../../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) have their own source contracts as well. The [module and file index above](#module-and-file-index) connects every definition to its explanatory chapter.

#### Compact routing and audit records

A probe hands over a decision about further work. The [Probe Profiles](../../framework/CognitiveTools_ProbeProfiles_v1.json) lite-audit contract requires `decision`, `confidence`, `expected_gain`, `kept_fields`, `suppressed_fields`, `suppression_reasons`, `escalation_reasons`, `dare_watchpoints` and `audit_stub`. The record should name the risk of suppression and its recheck trigger. Scores in these fields need an interpretation and grounds; merely emitting numbers does not measure benefit or confidence.

When CEC is active, preserve its `path_packet`, `dependency_graph` and `gap_report`. CREM can add its `crem_packet`, `rebase_vector` and `crem_gate_report`. DARE/IDCM can add `dare_audit_report`, `rescued_branch_refs`, `rerun_requests` and `operator_injection_requests`. Optional runtime observation can add `exec_trace`, `hidden_state_watch`, `fail_safe_report` and `runtime_parameters` when an application supplies the actual instruments. These are conditional handoff products; the task determines which contribution is active.

### Check whether the handoff can be used

The archive's receiving component needs to distinguish “the copy is adequate” from “inspect whether the copy is adequate.” Both sentences can occupy a plausible-looking field. Their different evidence status changes what the application may recommend.

A receiving check therefore has two parts. Parsing establishes whether the record can be read. Semantic review establishes what its claims are grounded in, which identifiers resolve, and whether the original scope and unresolved conditions remain intact.

The same distinction applies to a validation result. A source template containing placeholder strings is a skeleton. Replacing those strings with values can produce well-formed JSON without establishing that every source requirement was met. Full use of a module checks its complete specification, required inputs, gates and output contract.

In the archive example, a useful receiving result preserves the open binding request and the uninspected copy. If a later inspection establishes adequacy for wording, the record can acquire that finding with its source. The earlier uncertainty remains part of how the decision developed rather than becoming a claim that the copy had always been known to suffice.

*Consistency checking* finds mismatched records. *Scope preservation* prevents one request's result from migrating into another. *Return-path evaluation* checks that the carried proposal still answers the opening concern. Their combination allows another component to act on a bounded result without inheriting an unsupported conclusion.

A bounded request can make that translation inspectable:

> Use the archive case to prepare selected-field handoff excerpts for the relevant modules. Preserve the original question, actor responsibilities, evidence requirements and unknown conditions. Resolve each local identifier, map the module products to the packet index's receiving vocabulary, and state what the receiving component can do next. Identify omitted fields whose absence would prevent full contract use. Keep a proposed check distinct from a completed finding.

## 3. Applying a method

The chapters develop ways to represent a problem, transform its relationships and organize useful methods. This appendix brings the working references together: describe the case, try a transfer, and distinguish what an illustration shows from what an actual use establishes.

The examples below are original illustrations. The separately linked evaluation supplies recorded outputs for particular tasks. Keep the source, proposed operation and resulting evidence available when adapting either to another application.

### Represent the case

O/D/R/O separates four related aspects of a description. It is a lexical structure, not an embedding format, and does not need a particular model to read it.

| Field | Meaning | Access-dependency example |
|---|---|---|
| Ontology | The entities, roles or relationship being described. | A competent practitioner and a separate controller of necessary access. |
| Dynamics | The process or relationship that produces or maintains a state. | The practitioner can diagnose the fault, while task completion still requires access controlled elsewhere. |
| Regime | Conditions under which that description holds. | The controlled access is necessary and no viable alternative is available. |
| Outcome | A supported or conditional consequence. | Completing this task remains dependent on the access controller. |

#### Outcome and destination

The final O is used as *outcome* in the evaluation and as *destination* in some memory and transformation contexts. A consumer must know which interpretation it is receiving.

- An **observed outcome** records evidence of what happened.
- A **predicted outcome** states what a hypothesis implies, with uncertainty.
- A **desired destination** states an authorized objective.

Keep these statuses explicit in the surrounding record. An intended result must not silently become an observed fact. The existing source packet formats are preserved; this documentation does not introduce a replacement schema.

#### Boundaries of the representation

O/D/R/O helps organize claims; it does not verify them. Preserve a source pointer, mark unknowns, and distinguish an extracted relationship from a proposed analogy. Do not infer motives from a structural description. A similar shape in another domain suggests a candidate method, not proof that the same explanation applies.

### Carry the relation into an application

#### What should transfer?

A concept is reusable when its governing relationship and necessary conditions survive a change of setting. The technician's name and the workshop's location may be incidental. The necessity and control of access are consequential.

“Skill never produces independence” loses the condition. Merely repeating the technician's story leaves the abstraction implicit. A useful statement is narrower: competence alone does not remove a dependency created by externally controlled necessary access.

In this example, control of access belongs in the dynamics, and the exclusivity and necessity of access qualify the regime. Those choices can be inspected and challenged. Different tasks may support more than one useful representation.

#### Extract a relationship without making it universal

**Source:** A repair team can diagnose a failed pump. Another organization alone can unlock the control cabinet required to repair it. No alternative access route is currently available.

**Method:** KCE, with the O/D/R/O distinctions.

**Candidate concept:** Technical competence does not remove dependence on a party that exclusively controls necessary access.

**Check:** The source supports diagnosis, not mastery of every repair. It does not establish refusal or hostile intent. A viable alternative access route would change this particular dependency.

Try supplying the source and method to a model, then inspect whether its concept preserves those qualifications. Compare against the same task without the method; keep all attempts.

#### Preserve disagreement while enabling action

**Situation:** Two groups share a maintenance system. One wants more control over upgrades; the other wants dependable shared operating standards. Both still need the maintenance system.

**Method:** Coupler and CREM, with comparison if several proposals remain viable.

**Candidate reframe:** Distinguish authority over an upgrade from responsibility for shared operating standards. Consider an arrangement that separates those decisions while retaining the shared maintenance dependency.

**Check:** The proposed distinction is a candidate, not an agreement already reached. Neither group's demand establishes that its preferred arrangement is feasible. Practical cooperation need not imply trust or resolution of the underlying dispute.

#### Guide an article's movement

**Task:** Write an analysis of a fictional infrastructure negotiation using only supplied facts.

**Contextual guidance:** Establish the shared objective; distinguish technical feasibility from approval authority; preserve the parties' different dependencies; develop a conditional proposal only after the diagnosis.

**Check:** Does the finished article follow the relevant relationships without inventing a withdrawal, a motive or a successful negotiation? Does it read as an article rather than as a list of control instructions?

The [KCE evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) supplies a concrete version of this experiment, including the Kissinger framework and a rubric. Consult its task files for exact model inputs and its separate review materials for scoring.

#### A compact trial instruction

> Use the supplied facts as evidence. Identify the governing relationship and the conditions under which it applies. Apply only the cognitive method relevant to the task. Give the requested answer, followed by a short record of the method used, preserved constraints and unresolved uncertainty. Do not invent numerical measurements or imply that a proposed check has been performed.

This instruction is a starting point. The source specifications offer fuller stage and handoff definitions when a task requires them.

## 4. Evidence and evaluation

### Distinguish illustration from evidence

The framework is an explicit method collection. Its documentation, implementation in another project, successful use on one task and general effectiveness are different kinds of evidence.

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) includes:

- Encoding exercises: passage to governing concept, O/D/R/O and limits.
- A decoding exercise: a supplied Kissinger analytical framework and fictional facts to a new article.
- Separate dimensions for overgeneralization, undergeneralization, fidelity, structural transfer, writing quality and control-material leakage.
- An example report comparing Sol 6.1 at low reasoning effort with Qwen 3.8 27B, Q4_K_M, with thinking disabled.

The article task receives a prepared framework; it does not consume the model's preceding extraction. The example report contains six encoding cases and one article case per model, with separate, identity-masked AI review. Its judgments are provisional and have not been human-calibrated. Different backends and settings are recorded. This is evidence about particular outputs, not a broad model ranking or validation of every framework module.

### Assess a new use

Use comparable task inputs and settings across ordinary instructions and structured-framework conditions. Define the scoring criteria before examining outputs. Keep all attempts, failures and uncertainty; use reviewers who do not know the tested condition where practical. Evaluate new cases, including cases where the method should be suppressed.

Check whether any improvement is due to the framework's structure, the additional task information or simply a larger context budget. Measure costs as well as output quality. Repeated trials and independent human review matter before making general claims.

### Instrumentation boundaries

The JSON source specifications contain conceptual scores, thresholds, telemetry fields and runtime-probe proposals. This documentation release does not supply the instruments required to measure latent instability, neural attention, divergence, reward or every named confidence signal. A model-generated number is not automatically such a measurement.

Likewise, a schema-valid packet establishes only a structural property. Its source claims, applicability and proposed actions still require independent checks. Do not convert agreement between model roles into independent evidence of truth.

## 5. Source and version notes

### Publication source

The `framework/` directory contains 23 JSON definitions and templates and one agent-facing skill guide from the `skills/cognitive-tools` package in `bounded-route-hyperagent`, source commit `dc6b7e536aeace455637fa22ce08edbbade712c4`. All 23 JSON files remain byte-preserved. The [manifest](../../SOURCE_MANIFEST.json) records the current files and their size and SHA-256 identities.

The original publication also included three usage guides and a historical CREM PDF under `framework/references/`. Their important content is now incorporated into the chapters and this reference section. The manifest retains their former identities and links to the preceding publication for source inspection. The separate quick guides and file index have likewise been consolidated into the book.

### Skill guide publication repair

The source guide's unquoted YAML description contained `design: the model`, which a YAML reader treated as a mapping delimiter. A folded scalar repairs that header while preserving the description wording. A subsequent navigation revision replaces its removed reference-directory pointers with Chapter 15 and this reference section. All other instruction text is retained.

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

[Previous: From a Useful Transformation to a Reusable Method](../chapters/19_FROM_TRANSFORMATION_TO_REUSABLE_METHOD.md) · [Book contents](../../README.md)
