# Sentence-Thought Vectors and the Framework

[Book contents](../../README.md) · [Foundations](01_OVERVIEW_AND_BASICS.md) · [Compound Transformations](02_WORKING_WITH_TRANSFORMATIONS.md)

[Overview and Basics](01_OVERVIEW_AND_BASICS.md) introduces the cognitive transformations through simple examples and their limits. The [book design](../BOOK_DESIGN.md) outlines the broader documentation structure.

The opening chapters examined transformations and their combinations. This chapter deconstructs the anatomy of a thought while those transformations are applied: identify what is involved, what happens, the conditions that govern it, and what is affected or reached.

**From searching across knowledge domains to preserving and applying the structure of a thought.**

Large language models can draw connections across disciplines, extract concepts and turn an abstract idea into a specific explanation or piece of writing. These abilities are not always used reliably. A model may settle on the first plausible framing, lose a qualification during abstraction, or produce fluent prose that no longer follows the intended concept.

This framework grew out of developing Alex, an AI collaborator intended to carry useful approaches between tasks. Its evolution followed three connected questions: **where should the model look, what structure should it preserve, and how can that structure become reusable?**

This repository publishes the methods and structured specifications behind that work. They can be read, supplied selectively as model context, or used to design a harness. The overview below introduces the representation and the methods that use it. The following four chapters develop ontology, dynamics, regime and coupling separately.

## 1. Prism: broaden the inquiry before closing it

The original Prism began with ontology: identifying the kinds of things and relationships involved in a problem. During the October–November 2025 period, that idea developed into a framework of **19 broad categories of human knowledge**. They served as lenses through which the same prompt could be examined.

The motivation was to make better use of the knowledge already available to an LLM. A question first framed as an engineering problem might also involve biology, economics, political authority or human behavior. The fundamental idea was that an answer to the prompt had a certain shape regarding its actions and constraints.  Through analogical reasoning, similarly shaped answers might exist in an unrelated domain, and its general concepts would transpose back to a coherent answer.  That answer could remain plausible within its opening discipline while missing a relationship another domain would reveal.

Prism therefore sought to delay premature search closure. It encouraged alternative framings and movement through relevant disciplines or coherent domains before committing to an answer. The aim was selective breadth: explore another perspective when it could change the analysis, then stop when further exploration ceased to help.

At this stage, the central contribution was a map of **where to search**. That map also raised a further question: when an idea moves between domains, what must remain intact?

## 2. Sentence-thought vectors: describe what must survive

By April 2026, in the author's reconstruction of the development, the representation had expanded into the **sentence-thought framework**. Ontology was joined by dynamics, regime and a second ontology representing the object or destination.

The organizing analogy was the structure of a sentence:

| Element | Sentence analogy | Role in the thought |
|---|---|---|
| **Ontology** | Subject or noun | The entity, system or relationship we begin with. |
| **Dynamical** | Action or verb | What it does, undergoes or maintains. |
| **Regime** | Modifiers and qualifying phrases | Conditions and constraints governing the relationship. |
| **Ontology: object or destination** | Object or resulting state | What is affected, related to or reached. |

This became **O/D/R/O**. The rationale was that language—the material from which LLMs learn—already expresses meaning through entities, actions, qualifications and their relationships. The grade school exercise of diagramming a sentence into decomposable elements is case and point of its explicit existence within an LLM.  But deeper abstraction lies in the latent spaces and various  concepts, also known as coherent domains.  As such, the same structure also underlies higher level language structure which builds paragraphs, sections, essays, chapters, and books.  These higher level abstractions are also decomposable into those same **O/D/R/O** elements.  Collections of these sentence-constructs form the attractor basin.  The framework makes those roles explicit and available for inspection. It is a semantic model, rather than a requirement that every language or sentence follow one grammatical order.

Each component can be analyzed and categorized independently, much as the original Prism organized ontology into broad knowledge domains. Search can then consider a particular process across different subjects, a shared destination reached by different routes, or a relationship whose applicability changes under a different regime.

The components must also remain connected. Consider the test assertions “Americans love freedom” and “Americans do not love freedom.” They share a subject, a relationship and an object, while negation changes what is asserted. In a pure vector numerical embedding, the two sentences are semantically similar and may be difficult to distinguish one sentence from the other.  In a regime-based encoding, the logical constraint qualifies the love relationship. A useful representation preserves that scope; denying love does not establish hatred.

This was the intended advantage over relying only on whole-sentence similarity: make the consequential parts of meaning separately searchable while preserving the thought they form together. Realizing that advantage requires faithful normalization and a search or applicability check that respects the relationships.

The final O is not automatically a desired outcome. It may be the object of a relationship, such as freedom in the example, or a destination state in a transformation. Current consumer schemas use names such as `outcome` and `destination`; their contracts determine the interpretation. See [the O/D/R/O guide](../ODRO.md) for the current distinctions between consequences and objectives.

## 3. KCE: elevate the concept without losing the thought

A structured description of one experience is not yet a reusable method. It may remain tied to its original people, objects or wording. **KCE—Key Concept Extraction or Elevation—**addresses that next problem: identify the governing concept, lift it to a useful level of generality, and preserve the relationships and conditions that make it applicable.

For example, a technician may know how to diagnose a pump but still depend on someone else to unlock the workshop. The transferable concept concerns the separation between capability and control of necessary access. “Skill never creates independence” overgeneralizes it; merely retelling the workshop story leaves the reusable relationship implicit.

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval), KCE was incorporated into the thought-vector capture procedure to capture Henry Kissinger's pattern into a relational database.  The various orientations may be searched to help find reusable concepts across different situations. The documented procedure selects a provisional concept anchor, limits abstraction, and records the governing operation, applicability conditions and failure boundaries. Categories provide routes to the concept; the preserved thought supplies what a later model must assess.

That distinction matters. Two records can occupy similar categories while asserting different relationships. A retrieved candidate must still be checked against the present problem. Broader discovery and precise applicability are complementary parts of the design.

The next step is **specification**: bring the generalized concept back into a particular situation and express it as useful analysis, action or prose. That introduces another opportunity for error. The model must adapt the concept without importing the old example's facts or losing its qualifications.

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) makes those abilities inspectable through extraction exercises, a Kissinger-framework writing task and a scoring rubric. Its example scorecard compares Sol 6.1 with Qwen 3.8 27B with thinking disabled. The current evaluation tests extraction and application separately, supplying the framework for the writing task.

The historical progression is therefore **broader inquiry → structured thought → reusable concept → specific application**. The dates here follow the author's reconstruction and surviving discussions; they describe the design's evolution, rather than a sequence of verified software releases.

## 4. Choose, explore, compare and check

Once a concept is preserved, another question follows: what should the model do with it? The later modules made different jobs explicit instead of leaving every transformation inside one broad instruction.

**CTR** names the available transformations and what they must preserve. **ETE** applies selected transformations to produce meaningfully different candidate systems. **PSPP** compares those candidates and records why a branch is selected, merged or deferred. The various modules and frameworks have evolved.  They are more educational than functional in nature, even though they are structured as JSON skills.  A useful exercise is to load a skill and have your LLM describe and discuss it.  It may stimulate ideas for development or incorporation into a project.

An earlier picture made the search easier to imagine: walk around a circle from a thesis to its opposing view, hold the tension when both reveal something important, then try a **YZ tilt** if movement around the same plane keeps returning to the same difficulty. In the [archive example](09_THE_CIRCLE_AND_THE_TILT.md), opening fragile notebooks and protecting them seem opposed until the inquiry distinguishes access to their words from access to the physical objects. That distinction creates new arrangements worth exploring; comparison determines whether any of them earns the name synthesis.

Three further concerns require different checks. **CREM** reframes relationships while preserving the parties' differences and shared dependencies. **CEC** checks whether consequential steps form a licensed path. **DARE/IDCM** asks whether the opening frame or rejected branches concealed something important.

The supporting controls address cost, observability and feedback: **probe profiles** select the smallest useful route, **Organ Atlas** describes optional monitoring surfaces, and **Reward Controller** bounds how observed results may influence future effort. Some of these ideas have antecedents in the 2025 Prism work.

These are methods a capable model may already perform through prompting. Their intended contribution is to make the choice, constraints and checks explicit and reusable. The [historical guide](../HISTORY.md) traces the surviving evidence; each linked page below explains its problem, purpose, evolution and an example.

## The cognitive methods

| Reader guide | Contribution | Original definition |
|---|---|---|
| **[KCE](../skills/KCE.md)** | Preserve a reusable concept through abstraction. | [v2.3 JSON](../../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) |
| **[CDP](04_ONTOLOGICAL_PRISM.md)** | Select domain lenses that can change the analysis. | [v1.2 JSON](../../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) |
| **[Dynamical Prism](05_DYNAMICAL_PRISM.md)** | Describe the processes behind a behavior label. | [Reduced-core JSON](../../framework/Dynamical_Prism_v1.2_ReducedCore.json) |
| **[Regime Field](06_REGIME_FIELD.md)** | Preserve the conditions governing those processes. | [Field](../../framework/Regime_Field_v0.1.json) / [profile](../../framework/CognitiveTools_RegimeProfile_v1.json) |
| **[Prism Coupler](07_PRISM_COUPLER.md)** | Bind actors, roles, processes and constraints. | [v1.5 JSON](../../framework/Prism_Coupler_v1.5_OntologyDynamicsRegime.json) |
| **[CTR](../skills/CTR.md)** | Choose transformations and their preservation checks. | [v2.1 JSON](../../framework/CTR_Parallax_v2.1_SplitTransformRegistry.json) |
| **[ETE](../skills/ETE.md)** | Explore transformations and retain candidate systems. | [v1.1 JSON](../../framework/ETE_v1.1_SplitLayerExplorationTransform.json) |
| **[CREM](../skills/CREM.md)** | Rebase relationships without erasing parties or dependencies. | [v1.3 JSON](../../framework/CREM_v1.3_SplitOntologyDynamicsRegime.json) |
| **[PSPP](../skills/PSPP.md)** | Compare candidates before choosing a conclusion. | [v5.0-lite JSON](../../framework/PSPP_v5.0_CandidateSystemComparator.json) |
| **[CEC](../skills/CEC.md)** | Check consequential causal and dependency steps. | [v1.1 JSON](../../framework/CEC_Parallax_v1.1_ConditionalPathValidator.json) |
| **[DARE/IDCM](../skills/DARE.md)** | Audit the frame, pruning and unexplained residue. | [v1.0 JSON](../../framework/DARE_IDCM_v1.0_ParallelSupervisoryLayer.json) |
| **[Probe profiles](../skills/PROBES.md)** | Decide when a fuller operation is worth its cost. | [Profiles JSON](../../framework/CognitiveTools_ProbeProfiles_v1.json) |
| **[Organ Atlas](../skills/ORGAN_ATLAS.md)** | Define optional probes and recovery posture. | [v0.3 template](../../framework/Organ_Atlas_Template_v0.3.json) |
| **[Reward Controller](../skills/REWARD.md)** | Keep bounded feedback under external evaluation. | [Contract JSON](../../framework/RewardController_ParallaxEngine.v1.json) |

Use the smallest useful combination. A clear, simple task may need none of them. The [file index](../MODULES.md) also links packet templates and reference documents.

## Attention steering in practice

Using all of the included stages simultaneously in practice can be quite paralyzing for an LLM as it can be resource intensive to perform exhaustive search of information through the model.  However, many frontier models can take the "main idea" or the strategy of the JSON algorithm and can get quite good of a result.  These cognitive skills are merely illustrative of the various transformations that a model can do.  Not all models can perform these with equal proficiency.

## What is included

- [The original framework package](../../framework/): its agent-facing `SKILL.md`, 23 JSON specifications/templates and four reference documents.
- [An O/D/R/O explanation](../ODRO.md), [module index](../MODULES.md) and [worked examples](../WORKED_EXAMPLES.md).
- [Module history and evidence trail](../HISTORY.md), with individual reader guides linked above.
- [Research notes and open questions](../MUSINGS.md), including a proposed abductive loop.
- [Source/version notes](../PROVENANCE.md) and a [file-hash manifest](../../SOURCE_MANIFEST.json).

The original package is preserved as a source snapshot. Its historical status labels and numerical controls are design declarations, not evidence of measured reliability. Some specifications refer to companion modules or instruments that are not included. The provenance notes explain these boundaries.

## Read, try, contribute

Start with a problem whose facts you can inspect. Select one method, state what should remain invariant, and compare the resulting output with your ordinary approach. Keep failures and counterexamples. A valid packet is useful bookkeeping; its claims still need evidence.

Reports are most useful when they include the task, model and settings, supplied method, actual output, and the specific improvement or failure observed. Please use synthetic or redistributable examples and keep private conversations, credentials and personal memory databases out of submissions.

Published under the [MIT License](../../LICENSE). The goal is to make the methods available for inspection, adaptation and independent testing.

[Previous: Compound Transformations](02_WORKING_WITH_TRANSFORMATIONS.md) · [Next: The Ontological Prism](04_ONTOLOGICAL_PRISM.md)
