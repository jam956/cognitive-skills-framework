# ETE: explore alternatives without losing the question

**Question:** What candidate systems emerge when we actually apply the selected transformations?

## The problem and the method

Asking for several answers can produce stylistic variations of the same assumption. Exploration needs alternatives that differ in a consequential relationship, condition or mechanism.

ETE specifies how to apply CTR's selected operations, construct candidate systems and retain their return paths. It records rejected branches and reasons so a later reviewer can examine what pruning removed. Bounded exploration should stop producing branches when they no longer add useful distinctions.

## Historical development

Earlier discussions used MPO and MetaDiagnostic roles for projection and diagnostic exploration. Recovered May 2, 2026 discussion consolidated their runtime responsibilities into ETE, separating the transform vocabulary from its application. CTR was the registry; ETE was the executor.

ETE v1.1, added in the May 6 source update, extends that division to the separated ontology, Dynamical Core and Regime Field. It can explore changing an operating condition without replacing the entire domain, or investigate a different process under the same constraints.

## Example and boundary

A stalled repair might involve missing competence, unavailable parts or controlled access. These are useful alternatives only when the facts leave them plausible. ETE should state what each candidate would explain and what evidence would distinguish it.

The publication contains the execution specification, not an autonomous search service. A model or harness must carry out the operations. More branches do not automatically mean better reasoning; [PSPP](PSPP.md) compares the survivors.

**Read:** [ETE v1.1 specification](../../framework/ETE_v1.1_SplitLayerExplorationTransform.json) · [packet template](../../framework/ETE_v1.1_PacketTemplate.json) · [CTR](CTR.md) · [evidence trail](../HISTORY.md#evidence-trail)
