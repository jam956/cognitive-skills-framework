# Cognitive Skills Framework

**A documented approach to steering an LLM's attention, reasoning and expression through explicit cognitive methods.**

Large language models can extract concepts, change perspective, construct analogies, compare explanations and adapt their writing. Those abilities are not equally reliable on every suitable task. An answer may sound persuasive while losing a condition, flattening competing interests, or reaching a conclusion before the evidence supports it.

This framework makes some of those operations explicit. It describes what a model should preserve, what it may transform, when a method applies, and how its result can be checked. The aim is to help an AI collaborator use its existing capabilities more deliberately and carry useful methods between tasks.

This repository publishes the documentation and structured specifications. You can read them, supply selected methods as context to a model, or use them to design your own harness. There is no bundled autonomous runtime or model-weight update.

## Why we developed it

The framework grew out of developing Alex, an AI collaborator intended to maintain continuity of approach across writing, engineering and conceptual work. Remembering a prior answer is only part of that task. A reusable method also needs its purpose, the relationships that make it work, its limits, and a way to recognize when it no longer fits.

We began describing these structures explicitly and using them to direct attention. Instead of asking only for a persuasive answer, we could ask which relationship must survive a change of setting, which constraints govern the available actions, or whether a proposed resolution has erased a real disagreement.

The resulting methods are modular. They are meant to guide reasoning and make its products inspectable. Their usefulness still depends on the model, task, supplied evidence and verification.

## Start with O/D/R/O

O/D/R/O is a compact way to describe a situation or transferable concept:

| Element | Question |
|---|---|
| **Ontology** | What kinds of things, actors, roles or relationships are involved? |
| **Dynamics** | What happens, changes or maintains the relationship? |
| **Regime** | Under which conditions and constraints does it operate? |
| **Outcome / destination** | What follows, or what state is the task trying to reach? |

For example, a trained technician can still depend on someone else who controls access to the workshop. Skill and access are different parts of the system. A useful abstraction preserves both, along with the condition that access is necessary and exclusively controlled.

The same representation can support extraction, reframing, comparison, writing and memory. A predicted outcome and a desired destination must remain distinguishable: wanting a result does not establish that it will occur. See [the O/D/R/O guide](docs/ODRO.md).

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
