# Module and file index

Start with the [reader overview](../README.md), then the [original skill guide](../framework/SKILL.md) when applying the methods. Load only the definitions relevant to the task.

The component names below link to concise skill guides: quick reminders, companion examples and brief development notes. The chapter links give the extended treatment. Use the [design history](../archive/HISTORY.md) for historical questions; it is optional to the conceptual reading route.

## Book route

The [book contents](../README.md) lead from [basic transformations](../docs/chapters/01_OVERVIEW_AND_BASICS.md) and [their combinations](../docs/chapters/02_WORKING_WITH_TRANSFORMATIONS.md) to [sentence-thought vectors](../docs/chapters/03_SENTENCE_THOUGHT_VECTORS.md). The four tool chapters develop the [Ontological Prism](../docs/chapters/04_ONTOLOGICAL_PRISM.md), [Dynamical Prism](../docs/chapters/05_DYNAMICAL_PRISM.md), [Regime Field](../docs/chapters/06_REGIME_FIELD.md), and [Prism Coupler](../docs/chapters/07_PRISM_COUPLER.md). The next group develops [KCE](../docs/chapters/08_KEY_CONCEPT_EXTRACTION.md), [the circle and the tilt](../docs/chapters/09_THE_CIRCLE_AND_THE_TILT.md), [ETE](../docs/chapters/10_EXPLORATION_TRANSFORM_ENGINE.md), and [PSPP](../docs/chapters/11_PARALLEL_SYSTEM_COMPARISON.md). [CREM](../docs/chapters/12_RELATIONSHIP_REBASE.md), [CEC](../docs/chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) and [DARE/IDCM](../docs/chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) develop rebase, path validity and process audit. [Probe Profiles](../docs/chapters/15_SELECTIVE_TOOL_ROUTING.md), [Organ Atlas](../docs/chapters/16_OBSERVATION_AND_RECOVERY.md) and [Reward Controller](../docs/chapters/17_AUDITOR_FEEDBACK_CONTROL.md) cover selective application and optional engineering support. The [CTR reference guide](skills/CTR.md) supports transformation choice when needed. The table below retains the source-file index.

[Chapter 19](../docs/chapters/19_FROM_TRANSFORMATION_TO_REUSABLE_METHOD.md) considers what turns a useful transformation into a reusable method. [O/D/R/O](../docs/appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#1-represent-the-case) supplies the compact representation reference, and the [worked examples](../docs/appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#2-carry-the-relation-into-an-application) offer other application settings. The further design questions are developed in [Chapter 18](../docs/chapters/18_OPEN_QUESTIONS_AND_FURTHER_DIRECTIONS.md).

## Definitions and controls

| Component / quick guide | Internal version | Role | Source | Book route |
|---|---|---|---|---|
| [KCE](skills/KCE.md) | `v2.3.0` | Identify provisional anchors and compression risks. | [Specification](../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) | [8](../docs/chapters/08_KEY_CONCEPT_EXTRACTION.md) |
| [CDP](skills/CDP.md) | `v1.2.0` | Select relevant domains and expose collision or lock-in risks. | [Specification](../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) | [4](../docs/chapters/04_ONTOLOGICAL_PRISM.md) |
| [Regime profile](skills/REGIME.md) | `v1.0.0` | Pass a compact constraint surface between stages. | [Specification](../framework/CognitiveTools_RegimeProfile_v1.json) | [6](../docs/chapters/06_REGIME_FIELD.md) |
| [Dynamical Prism](skills/DYNAMICAL.md) | `v0.2.0_reduced_core` | Describe primitive processes separately from conditions. | [Specification](../framework/Dynamical_Prism_v1.2_ReducedCore.json) | [5](../docs/chapters/05_DYNAMICAL_PRISM.md) |
| [Regime Field](skills/REGIME.md) | `v0.1.0` | Describe constraints, operating conditions and phase. | [Specification](../framework/Regime_Field_v0.1.json) | [6](../docs/chapters/06_REGIME_FIELD.md) |
| [Coupler](skills/COUPLER.md) | `v1.5.0` | Bind ontology, actors, processes and regime. | [Specification](../framework/Prism_Coupler_v1.5_OntologyDynamicsRegime.json) | [7](../docs/chapters/07_PRISM_COUPLER.md) |
| [CTR](skills/CTR.md) | `v2.1.0` | Select transformations and preservation checks. | [Specification](../framework/CTR_Parallax_v2.1_SplitTransformRegistry.json) | [Reference](skills/CTR.md) |
| [ETE](skills/ETE.md) | `v1.1.0` | Explore selected transformations and retain candidate branches. | [Specification](../framework/ETE_v1.1_SplitLayerExplorationTransform.json) | [10](../docs/chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) |
| [CREM](skills/CREM.md) | `v1.3.0` | Rebase conflict and alignment while preserving dependencies. | [Specification](../framework/CREM_v1.3_SplitOntologyDynamicsRegime.json) | [12](../docs/chapters/12_RELATIONSHIP_REBASE.md) |
| [PSPP](skills/PSPP.md) | `v5.0.0-lite` | Compare and select, merge or defer candidates. | [Specification](../framework/PSPP_v5.0_CandidateSystemComparator.json) | [11](../docs/chapters/11_PARALLEL_SYSTEM_COMPARISON.md) |
| [CEC](skills/CEC.md) | `v1.1.0` | Validate consequential ordering and dependency gaps. | [Specification](../framework/CEC_Parallax_v1.1_ConditionalPathValidator.json) | [13](../docs/chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) |
| [DARE/IDCM](skills/DARE.md) | `v1.0.0` | Audit closure, pruning, missing operators and fragility. | [Specification](../framework/DARE_IDCM_v1.0_ParallelSupervisoryLayer.json) | [14](../docs/chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) |
| [Probe profiles](skills/PROBES.md) | `v1.0.0` | Choose a small sufficient route before loading full definitions. | [Specification](../framework/CognitiveTools_ProbeProfiles_v1.json) | [15](../docs/chapters/15_SELECTIVE_TOOL_ROUTING.md) |
| [Organ Atlas](skills/ORGAN_ATLAS.md) | `not declared` | Describe optional monitoring and fail-safe probes; instruments are external. | [Specification](../framework/Organ_Atlas_Template_v0.3.json) | [16](../docs/chapters/16_OBSERVATION_AND_RECOVERY.md) |
| [Reward Controller](skills/REWARD.md) | `1.0` | Specify auditor-owned future feedback, not autonomous reward optimization. | [Specification](../framework/RewardController_ParallaxEngine.v1.json) | [17](../docs/chapters/17_AUDITOR_FEEDBACK_CONTROL.md) |

## Packet templates

These are handoff skeletons. They are not transcripts of hidden reasoning or evidence that a model performed a check. [Appendix A](../docs/appendices/A_STRUCTURED_HANDOFFS.md) supplies worked selected-field examples and explains how their products map to the receiving vocabulary.

- [CREM_v1.3_PacketTemplate.json](../framework/CREM_v1.3_PacketTemplate.json)
- [CTR_Parallax_v2.1_PacketTemplate.json](../framework/CTR_Parallax_v2.1_PacketTemplate.json)
- [CognitiveTools_PacketTemplateIndex_v1.json](../framework/CognitiveTools_PacketTemplateIndex_v1.json)
- [Dynamical_Prism_v0.2_PacketTemplate.json](../framework/Dynamical_Prism_v0.2_PacketTemplate.json)
- [ETE_v1.1_PacketTemplate.json](../framework/ETE_v1.1_PacketTemplate.json)
- [KCE_Parallax_v2.3_PacketTemplate.json](../framework/KCE_Parallax_v2.3_PacketTemplate.json)
- [Prism_Coupler_v1.5_PacketTemplate.json](../framework/Prism_Coupler_v1.5_PacketTemplate.json)
- [Regime_Field_v0.1_PacketTemplate.json](../framework/Regime_Field_v0.1_PacketTemplate.json)

## Reference guides

- [CREM_Pipeline_Document_v1.pdf](../framework/references/CREM_Pipeline_Document_v1.pdf)
- [cognitive-tools-architecture.md](../framework/references/cognitive-tools-architecture.md)
- [cognitive-tools-file-map.md](../framework/references/cognitive-tools-file-map.md)
- [cognitive-tools-probe-strategy.md](../framework/references/cognitive-tools-probe-strategy.md)

The architecture and file map describe selective ordering and historical filenames. Read [source and version notes](PROVENANCE.md) before treating a status label, optional telemetry field or external companion as an implemented capability.
