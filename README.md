# Cognitive Skills Framework

**From searching across knowledge domains to preserving and applying the structure of a thought.**

Large language models can draw connections across disciplines, extract concepts and turn an abstract idea into a specific explanation or piece of writing. These abilities are not always used reliably. A model may settle on the first plausible framing, lose a qualification during abstraction, or produce fluent prose that no longer follows the intended concept.

This framework grew out of developing Alex, an AI collaborator intended to carry useful approaches between tasks. Its evolution followed three connected questions: **where should the model look, what structure should it preserve, and how can that structure become reusable?**

This repository publishes the methods and structured specifications behind that work. They can be read, supplied selectively as model context, or used to design a harness. The historical progression below explains their purpose before introducing the individual modules.

## 1. Prism: broaden the inquiry before closing it

The original Prism began with ontology: identifying the kinds of things and relationships involved in a problem. During the October–November 2025 period, that idea developed into a framework of **19 broad categories of human knowledge**. They served as lenses through which the same prompt could be examined.

The motivation was to make better use of the knowledge already available to an LLM. A question first framed as an engineering problem might also involve biology, economics, political authority or human behavior. An answer could remain plausible within its opening discipline while missing a relationship another domain would reveal.

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

This became **O/D/R/O**. The rationale was that language—the material from which LLMs learn—already expresses meaning through entities, actions, qualifications and their relationships. The framework makes those roles explicit and available for inspection. It is a semantic model, rather than a requirement that every language or sentence follow one grammatical order.

Each component can be analyzed and categorized independently, much as the original Prism organized ontology into broad knowledge domains. Search can then consider a particular process across different subjects, a shared destination reached by different routes, or a relationship whose applicability changes under a different regime.

The components must also remain connected. Consider the test assertions “Americans love freedom” and “Americans do not love freedom.” They share a subject, a relationship and an object, while negation changes what is asserted. In a regime-based encoding, the logical constraint qualifies the love relationship. A useful representation preserves that scope; denying love does not establish hatred.

This was the intended advantage over relying only on whole-sentence similarity: make the consequential parts of meaning separately searchable while preserving the thought they form together. Realizing that advantage requires faithful normalization and a search or applicability check that respects the relationships.

The final O is not automatically a desired outcome. It may be the object of a relationship, such as freedom in the example, or a destination state in a transformation. Current consumer schemas use names such as `outcome` and `destination`; their contracts determine the interpretation. See [the O/D/R/O guide](docs/ODRO.md) for the current distinctions between consequences and objectives.

## 3. KCE: elevate the concept without losing the thought

A structured description of one experience is not yet a reusable method. It may remain tied to its original people, objects or wording. **KCE—Key Concept Extraction or Elevation—**addresses that next problem: identify the governing concept, lift it to a useful level of generality, and preserve the relationships and conditions that make it applicable.

For example, a technician may know how to diagnose a pump but still depend on someone else to unlock the workshop. The transferable concept concerns the separation between capability and control of necessary access. “Skill never creates independence” overgeneralizes it; merely retelling the workshop story leaves the reusable relationship implicit.

In Basin Memory, KCE was incorporated into capture and search orientation to help find reusable concepts across different situations. The documented procedure selects a provisional concept anchor, limits abstraction, and records the governing operation, applicability conditions and failure boundaries. Categories provide routes to the concept; the preserved thought supplies what a later model must assess.

That distinction matters. Two records can occupy similar categories while asserting different relationships. A retrieved candidate must still be checked against the present problem. Broader discovery and precise applicability are complementary parts of the design.

The next step is **specification**: bring the generalized concept back into a particular situation and express it as useful analysis, action or prose. That introduces another opportunity for error. The model must adapt the concept without importing the old example's facts or losing its qualifications.

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) makes those abilities inspectable through extraction exercises, a Kissinger-framework writing task and a scoring rubric. Its example scorecard compares Sol 6.1 with Qwen 3.8 27B with thinking disabled. The current evaluation tests extraction and application separately, supplying the framework for the writing task.

The historical progression is therefore **broader inquiry → structured thought → reusable concept → specific application**. The dates here follow the author's reconstruction and surviving discussions; they describe the design's evolution, rather than a sequence of verified software releases.

## The cognitive methods

| Method | Contribution |
|---|---|
| **KCE — key concept extraction/elevation** | Finds provisional anchors and preserves relationships through abstraction. |
| **CDP — Cognitive Domain Prism** | Selects relevant domain lenses and limits unnecessary breadth. |
| **Dynamical Prism and Regime Field** | Separates actions and processes from their operating conditions. |
| **Prism Coupler** | Binds actors, roles, actions and conditions into a candidate system. |
| **CTR — Cognitive Transformation Registry** | Selects transformations and states what they preserve and disturb. |
| **ETE — Exploration and Transform Engine** | Explores candidate transformations and retains useful alternatives. |
| **CREM — Conflict and Relationship Rebase Module** | Reframes relationships while preserving consequential differences and dependencies. |
| **PSPP — candidate-system comparison** | Compares, selects, merges or defers candidate systems. |
| **CEC — conditional path validation** | Checks ordered dependencies when sequence matters. |
| **DARE/IDCM — supervisory audit** | Challenges premature closure, missing operations and unexplained residue. |
| **Probe profiles, Organ Atlas and Reward Controller** | Specify selective routing, optional monitoring and bounded feedback. |

Use the smallest useful combination. A clear, simple task may need none of them. See the [module and file index](docs/MODULES.md) for definitions, versions and entry points.

## Attention steering in practice

A short prompt can name a desired result while leaving the model to choose the route. Structured context can also describe the route: what to notice, which relationships to preserve, which transformations are permitted, and when to stop or reconsider.

In an analytical article, that might mean moving from a shared aspiration through conflicting dependencies to a conditional proposal. In a disagreement, it might mean recognizing that practical cooperation does not require restored trust. In memory, it might mean retaining the conditions under which a previous method can transfer.

Here, **attention steering means contextual guidance of the model's observable work**. The framework does not expose or directly manipulate neural attention weights. A matched evaluation is needed to establish improvement over a simpler prompt. The [worked examples](docs/WORKED_EXAMPLES.md) show how to try the methods without assuming that improvement in advance.

## Applications and evidence

- **[Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval)** tests concept extraction and application of a supplied analytical framework. It includes a normalized Kissinger corpus, scoring rubric and an example Sol 6.1 versus Qwen 3.8 27B comparison. The scores are provisional AI judgments and assess selected abilities, not this entire framework.
- **[Basin Memory](https://github.com/jam956/basin-memory)** applies a reduced cognitive tool set to reusable conceptual memory, applicability boundaries and provenance. Access depends on that repository's visibility.
- **Noetic Cortex** is related work on perception, motivation, attention and expression. Its runtime and personal/project databases are outside this documentation release.

These applications offer ways to examine the methods. Their existence does not establish that every module is effective. See [evaluation and limitations](docs/EVALUATION.md).

## What is included

- [The original framework package](framework/): its agent-facing `SKILL.md`, 23 JSON specifications/templates and four reference documents.
- [An O/D/R/O explanation](docs/ODRO.md), [module index](docs/MODULES.md) and [worked examples](docs/WORKED_EXAMPLES.md).
- [Research notes and open questions](docs/MUSINGS.md), including a proposed abductive loop.
- [Source/version notes](docs/PROVENANCE.md) and a [file-hash manifest](SOURCE_MANIFEST.json).

The original package is preserved as a source snapshot. Its historical status labels and numerical controls are design declarations, not evidence of measured reliability. Some specifications refer to companion modules or instruments that are not included. The provenance notes explain these boundaries.

## Read, try, contribute

Start with a problem whose facts you can inspect. Select one method, state what should remain invariant, and compare the resulting output with your ordinary approach. Keep failures and counterexamples. A valid packet is useful bookkeeping; its claims still need evidence.

Reports are most useful when they include the task, model and settings, supplied method, actual output, and the specific improvement or failure observed. Please use synthetic or redistributable examples and keep private conversations, credentials and personal memory databases out of submissions.

Published under the [MIT License](LICENSE). The goal is to make the methods available for inspection, adaptation and independent testing.
