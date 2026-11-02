# Structured Handoffs and Packet Examples

A comparison has selected a reproduction for one research request and left another request unresolved. The next component needs enough of that decision to answer correctly. “Use copies” loses the request, the adequacy check and the remaining need for original examination. Carrying every exploratory note would make the useful distinction harder to recover.

A handoff preserves the relationships the next act depends on. The packet templates provide places to record them. Their value appears when a receiving component can continue the work without inventing a missing condition or repeating the whole inquiry.

## 1. Decide what the receiver needs

For the archive, a useful handoff identifies the request, the feature it requires, the proposed carrier, the result of any actual check, and what remains unknown. A binding question must not inherit a decision made for wording simply because both concern the same notebook.

*Decomposition* separates the request from its carrier and conditions. *Relation extraction* keeps their dependencies explicit. *Scope preservation* attaches a finding to the case it supports. Together they make a compact record possible without reducing it to an unsupported conclusion.

The [packet index](../../framework/CognitiveTools_PacketTemplateIndex_v1.json) names a thin common vocabulary, including `anchor`, `regime_profile`, `dynamical_profile`, `coupling_packet`, `transform_plan`, `branch_set` and `return_path`. A richer module record can preserve additional detail when it matters. The index's default is to load the relevant template selectively.

The examples below are **selected-field excerpts** from an illustrative archive case. Each block is valid JSON and uses the corresponding source record's field names. It omits parts of the full contract; it is not a complete execution result or a conformance fixture. Where a template leaves an array's item shape open, the example supplies small application records. The identifiers `A1`, `R1`, `B_copy` and `RP1` are local example references.

Unknown inspection results remain unknown. Numerical defaults in the templates are not filled merely to make an excerpt look complete.

## 2. Choose the record for the work being carried

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
| Organ Atlas | `not declared` | Describe optional monitoring and fail-safe probes; instruments are external. | [Specification](../../framework/Organ_Atlas_Template_v0.3.json) | [16](../chapters/16_OBSERVATION_AND_RECOVERY.md) |
| Reward Controller | `1.0` | Specify auditor-owned future feedback, not autonomous reward optimization. | [Specification](../../framework/RewardController_ParallaxEngine.v1.json) | [17](../chapters/17_AUDITOR_FEEDBACK_CONTROL.md) |

## 3. Follow one case through the template fields

### KCE: retain the governing relationship

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

### Dynamical Prism: preserve what is being done

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

### Regime Field: keep missing conditions visible

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

### Coupler: connect responsibility to a permitted action

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

### CTR: retain the purpose of the movement

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

### ETE: make the alternative conditional in a useful way

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

### CREM: preserve the parties while proposing a changed relationship

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

## 4. Translate into the receiving vocabulary

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

### Compact routing and audit records

A probe hands over a decision about further work. The [Probe Profiles](../../framework/CognitiveTools_ProbeProfiles_v1.json) lite-audit contract requires `decision`, `confidence`, `expected_gain`, `kept_fields`, `suppressed_fields`, `suppression_reasons`, `escalation_reasons`, `dare_watchpoints` and `audit_stub`. The record should name the risk of suppression and its recheck trigger. Scores in these fields need an interpretation and grounds; merely emitting numbers does not measure benefit or confidence.

When CEC is active, preserve its `path_packet`, `dependency_graph` and `gap_report`. CREM can add its `crem_packet`, `rebase_vector` and `crem_gate_report`. DARE/IDCM can add `dare_audit_report`, `rescued_branch_refs`, `rerun_requests` and `operator_injection_requests`. Optional runtime observation can add `exec_trace`, `hidden_state_watch`, `fail_safe_report` and `runtime_parameters` when an application supplies the actual instruments. These are conditional handoff products; the task determines which contribution is active.

## 5. Check whether the handoff can be used

The archive's receiving component needs to distinguish “the copy is adequate” from “inspect whether the copy is adequate.” Both sentences can occupy a plausible-looking field. Their different evidence status changes what the application may recommend.

A receiving check therefore has two parts. Parsing establishes whether the record can be read. Semantic review establishes what its claims are grounded in, which identifiers resolve, and whether the original scope and unresolved conditions remain intact.

The same distinction applies to a validation result. A source template containing placeholder strings is a skeleton. Replacing those strings with values can produce well-formed JSON without establishing that every source requirement was met. Full use of a module checks its complete specification, required inputs, gates and output contract.

In the archive example, a useful receiving result preserves the open binding request and the uninspected copy. If a later inspection establishes adequacy for wording, the record can acquire that finding with its source. The earlier uncertainty remains part of how the decision developed rather than becoming a claim that the copy had always been known to suffice.

*Consistency checking* finds mismatched records. *Scope preservation* prevents one request's result from migrating into another. *Return-path evaluation* checks that the carried proposal still answers the opening concern. Their combination allows another component to act on a bounded result without inheriting an unsupported conclusion.

A bounded request can make that translation inspectable:

> Use the archive case to prepare selected-field handoff excerpts for the relevant modules. Preserve the original question, actor responsibilities, evidence requirements and unknown conditions. Resolve each local identifier, map the module products to the packet index's receiving vocabulary, and state what the receiving component can do next. Identify omitted fields whose absence would prevent full contract use. Keep a proposed check distinct from a completed finding.

Reference: [packet template index](../../framework/CognitiveTools_PacketTemplateIndex_v1.json) · [module and file index](A_STRUCTURED_HANDOFFS.md#module-and-file-index) · [source and version notes](B_APPLYING_AND_ASSESSING_A_METHOD.md#6-source-and-version-notes).

[Previous: From a Useful Transformation to a Reusable Method](../chapters/19_FROM_TRANSFORMATION_TO_REUSABLE_METHOD.md) · [Next: Applying and Assessing a Method](B_APPLYING_AND_ASSESSING_A_METHOD.md) · [Book contents](../../README.md)
