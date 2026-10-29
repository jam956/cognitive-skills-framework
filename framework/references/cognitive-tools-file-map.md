# Cognitive Tools File Map

Use this map to load the smallest relevant artifact first.

## Start Here

- `SKILL.md`
  Agent-facing usage rules, canonical packet vocabulary, and insertion policy.
- `references/cognitive-tools-architecture.md`
  Route table, operational order, and handoff boundaries.
- `references/cognitive-tools-probe-strategy.md`
  Probe-first routing strategy for efficient stack selection.
- `CognitiveTools_ProbeProfiles_v1.json`
  Machine-readable probe profiles, stack presets, and compact handoff contract.
- `CognitiveTools_PacketTemplateIndex_v1.json`
  Index for optional full-mode packet templates. Load this before any
  `*_PacketTemplate.json` file, and only load the template for the module being
  fully executed.

## Current Engine Specs

- `KCE_Parallax_v2.3_SplitLayerAnchor.json`
  Provisional anchor extraction with separate ontology, dynamical-core,
  regime-field, actor-role, computed-label, and transform seed candidates.
- `CDP_Parallax_v1.2_BoundedDomainSpace.json`
  Bounded 19-domain projection, candidate-specific prism profiles, breadth
  budgeting, collision risks, and domain-lock signals.
- `CognitiveTools_RegimeProfile_v1.json`
  Lightweight handoff spec emitted between CDP and Dynamical Prism. It carries
  the regime constraint surface, operator modulation, shift triggers, and DARE
  watchpoints without becoming a full reasoning engine.
- `Dynamical_Prism_v1.2_ReducedCore.json`
  Reduced primitive action verbs and computed behavior-label policy. Regime
  constraints live in `Regime_Field_v0.1.json`.
- `Regime_Field_v0.1.json`
  Explicit context, phase, constraint, threshold, legitimacy, trust, and
  operating-condition axes that modify primitive action vectors.
- `Prism_Coupler_v1.5_OntologyDynamicsRegime.json`
  Actor-role-regime binding, relationship edge detection, CREM-ready handoff,
  and post-Coupler route gate.
- `CTR_Parallax_v2.1_SplitTransformRegistry.json`
  Central transformation family/operator registry and verification/return-path
  requirements.
- `ETE_v1.1_SplitLayerExplorationTransform.json`
  Bounded exploration, operator-level projection, branch discovery, projection
  ledger, and rejected-branch artifacts for DARE inspection.
- `CREM_v1.3_SplitOntologyDynamicsRegime.json`
  N-party conflict, alignment, relationship repair, coalition, and dependency
  rebase logic.
- `PSPP_v5.0_CandidateSystemComparator.json`
  Lite candidate-system comparison, pruning, merge/select decisions, and audit
  artifacts.
- `CEC_Parallax_v1.1_ConditionalPathValidator.json`
  Conditional path validity, dependency unrolling, missing-middle audit, and
  ordered path packet emission.
- `DARE_IDCM_v1.0_ParallelSupervisoryLayer.json`
  Parallel supervisory audit, branch rescue, false harmony detection, operator
  gap detection, and bounded discontinuous anchor reconstitution.
- `RewardController_ParallaxEngine.v1.json`
  Auditor-owned bounded feedback controller. It consumes MPE/DARE/process
  signals and emits future-assignment dial nudges without becoming an
  inner-agent objective.

## Retired Specs

These older specs are intentionally retired from the active package. Their
successors carry `supersedes` metadata so loaders and reviewers can trace the
rename without resolving the retired files:

- `KCE_Parallax_v2.2_ProvisionalAnchor.json` -> `KCE_Parallax_v2.3_SplitLayerAnchor.json`
- `Dynamical Prism V1.JSON` -> `Dynamical_Prism_v1.2_ReducedCore.json`
- `Dynamical_Prism_EXEC_Process V1.py` -> reduced-core runtime probe in `Dynamical_Prism_v1.2_ReducedCore.json` plus `Organ_Atlas_Template_v0.3.json`
- `Prism_Coupler_v1.4_CREMRouteGate.json` -> `Prism_Coupler_v1.5_OntologyDynamicsRegime.json`
- `CTR_Parallax_v2.0_OperatorRegistry.json` -> `CTR_Parallax_v2.1_SplitTransformRegistry.json`
- `ETE_ExplorationTransformEngine_v1.0.json` -> `ETE_v1.1_SplitLayerExplorationTransform.json`
- `CREM_v1.2_NPartyRelationshipRebase.json` -> `CREM_v1.3_SplitOntologyDynamicsRegime.json`

## Executable Supports

- `Dynamical_Prism_v1.2_ReducedCore.json`
  Source for reduced-core runtime probe packets when instability or hidden-state
  watchpoints must be attached.
- `Organ_Atlas_Template_v0.3.json`
  Optional hidden-state and fail-safe scaffold for executable dynamical probing.
- `references/CREM_Pipeline_Document_v1.pdf`
  Human-readable CREM reference document when prose detail is needed.

## Packet Templates

- `KCE_Parallax_v2.3_PacketTemplate.json`
  Full anchor and split-layer seed skeleton.
- `Dynamical_Prism_v0.2_PacketTemplate.json`
  Full reduced-core operator-vector skeleton with canonical
  `dynamical_profile` mirror.
- `Regime_Field_v0.1_PacketTemplate.json`
  Full regime skeleton with canonical `regime_profile` mirror.
- `Prism_Coupler_v1.5_PacketTemplate.json`
  Full actor-role-regime binding skeleton with canonical `coupling_packet`
  mirror.
- `CTR_Parallax_v2.1_PacketTemplate.json`
  Full transform-plan skeleton.
- `ETE_v1.1_PacketTemplate.json`
  Full exploration and branch-emission skeleton.
- `CREM_v1.3_PacketTemplate.json`
  Full relationship-rebase skeleton.

## Loading Rule

Load `SKILL.md` first. Load the probe strategy next when deciding stack shape.
Load `CognitiveTools_ProbeProfiles_v1.json` for machine-readable routing.
Load `CognitiveTools_PacketTemplateIndex_v1.json` only when full module output
needs a template. Load full engine specs only after a probe returns
`escalate_full` or the user explicitly asks to inspect a full module.
