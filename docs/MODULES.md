# Module and file index

Start with the [reader overview](../README.md), then the [original skill guide](../framework/SKILL.md) when applying the methods. Load only the definitions relevant to the task.

The component names below link to concise skill guides: quick reminders, companion examples and brief development notes. The chapter links give the extended treatment. Use the [design history](HISTORY.md) for historical questions; it is optional to the conceptual reading route.

## Textbook route

The [book contents](../README.md) lead from [basic transformations](chapters/01_OVERVIEW_AND_BASICS.md) and [their combinations](chapters/02_WORKING_WITH_TRANSFORMATIONS.md) to [sentence-thought vectors](chapters/03_SENTENCE_THOUGHT_VECTORS.md). The four tool chapters develop the [Ontological Prism](chapters/04_ONTOLOGICAL_PRISM.md), [Dynamical Prism](chapters/05_DYNAMICAL_PRISM.md), [Regime Field](chapters/06_REGIME_FIELD.md), and [Prism Coupler](chapters/07_PRISM_COUPLER.md). The next group develops [KCE](chapters/08_KEY_CONCEPT_EXTRACTION.md), [the circle and the tilt](chapters/09_THE_CIRCLE_AND_THE_TILT.md), [ETE](chapters/10_EXPLORATION_TRANSFORM_ENGINE.md), and [PSPP](chapters/11_PARALLEL_SYSTEM_COMPARISON.md). [CREM](chapters/12_RELATIONSHIP_REBASE.md), [CEC](chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) and [DARE/IDCM](chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) develop rebase, path validity and process audit. [Probe Profiles](chapters/15_SELECTIVE_TOOL_ROUTING.md), [Organ Atlas](chapters/16_OBSERVATION_AND_RECOVERY.md) and [Reward Controller](chapters/17_AUDITOR_FEEDBACK_CONTROL.md) cover selective application and optional engineering support. The [CTR reference guide](skills/CTR.md) supports transformation choice when needed. The table below retains the source-file index.

The [afterword](AFTERWORD.md) considers what turns a useful transformation into a reusable method. [O/D/R/O](ODRO.md) supplies the compact representation reference, and the [worked examples](WORKED_EXAMPLES.md) offer other application settings. The remaining research questions stay in the [notebook](MUSINGS.md).

## Definitions and controls

| Component / quick guide | Internal version | Role | Source | Book route |
|---|---|---|---|---|
| [KCE](skills/KCE.md) | `v2.3.0` | Identify provisional anchors and compression risks. | [Specification](../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) | [8](chapters/08_KEY_CONCEPT_EXTRACTION.md) |
| [CDP](skills/CDP.md) | `v1.2.0` | Select relevant domains and expose collision or lock-in risks. | [Specification](../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) | [4](chapters/04_ONTOLOGICAL_PRISM.md) |
| [Regime profile](skills/REGIME.md) | `v1.0.0` | Pass a compact constraint surface between stages. | [Specification](../framework/CognitiveTools_RegimeProfile_v1.json) | [6](chapters/06_REGIME_FIELD.md) |
| [Dynamical Prism](skills/DYNAMICAL.md) | `v0.2.0_reduced_core` | Describe primitive processes separately from conditions. | [Specification](../framework/Dynamical_Prism_v1.2_ReducedCore.json) | [5](chapters/05_DYNAMICAL_PRISM.md) |
| [Regime Field](skills/REGIME.md) | `v0.1.0` | Describe constraints, operating conditions and phase. | [Specification](../framework/Regime_Field_v0.1.json) | [6](chapters/06_REGIME_FIELD.md) |
| [Coupler](skills/COUPLER.md) | `v1.5.0` | Bind ontology, actors, processes and regime. | [Specification](../framework/Prism_Coupler_v1.5_OntologyDynamicsRegime.json) | [7](chapters/07_PRISM_COUPLER.md) |
| [CTR](skills/CTR.md) | `v2.1.0` | Select transformations and preservation checks. | [Specification](../framework/CTR_Parallax_v2.1_SplitTransformRegistry.json) | [Reference](skills/CTR.md) |
| [ETE](skills/ETE.md) | `v1.1.0` | Explore selected transformations and retain candidate branches. | [Specification](../framework/ETE_v1.1_SplitLayerExplorationTransform.json) | [10](chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) |
| [CREM](skills/CREM.md) | `v1.3.0` | Rebase conflict and alignment while preserving dependencies. | [Specification](../framework/CREM_v1.3_SplitOntologyDynamicsRegime.json) | [12](chapters/12_RELATIONSHIP_REBASE.md) |
| [PSPP](skills/PSPP.md) | `v5.0.0-lite` | Compare and select, merge or defer candidates. | [Specification](../framework/PSPP_v5.0_CandidateSystemComparator.json) | [11](chapters/11_PARALLEL_SYSTEM_COMPARISON.md) |
| [CEC](skills/CEC.md) | `v1.1.0` | Validate consequential ordering and dependency gaps. | [Specification](../framework/CEC_Parallax_v1.1_ConditionalPathValidator.json) | [13](chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) |
| [DARE/IDCM](skills/DARE.md) | `v1.0.0` | Audit closure, pruning, missing operators and fragility. | [Specification](../framework/DARE_IDCM_v1.0_ParallelSupervisoryLayer.json) | [14](chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) |
| [Probe profiles](skills/PROBES.md) | `v1.0.0` | Choose a small sufficient route before loading full definitions. | [Specification](../framework/CognitiveTools_ProbeProfiles_v1.json) | [15](chapters/15_SELECTIVE_TOOL_ROUTING.md) |
| [Organ Atlas](skills/ORGAN_ATLAS.md) | `not declared` | Describe optional monitoring and fail-safe probes; instruments are external. | [Specification](../framework/Organ_Atlas_Template_v0.3.json) | [16](chapters/16_OBSERVATION_AND_RECOVERY.md) |
| [Reward Controller](skills/REWARD.md) | `1.0` | Specify auditor-owned future feedback, not autonomous reward optimization. | [Specification](../framework/RewardController_ParallaxEngine.v1.json) | [17](chapters/17_AUDITOR_FEEDBACK_CONTROL.md) |

## Packet templates

These are handoff skeletons. They are not transcripts of hidden reasoning or evidence that a model performed a check. [Appendix A](appendices/A_STRUCTURED_HANDOFFS.md) supplies worked selected-field examples and explains how their products map to the receiving vocabulary.

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
