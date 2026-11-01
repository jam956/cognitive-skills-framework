# A Textbook for Designing with Cognitive Transformations

**Working editorial design · revised 31 October 2026**

This book explains the ideas behind the Cognitive Skills Framework so that a program designer can develop an application of their own. The repository's modules are examples of ways to organize an LLM's abilities. They provide useful distinctions and possible designs within a much larger space of approaches.

The main reading path follows conceptual prerequisites. Development history and detailed evaluation remain supporting reference. The first chapter establishes what transformations a model may be capable of, how it can use information, and why those capacities offer possibilities for application design.

The narrative stance is collegial exposition. The prose lays out cases, relationships and consequences for a technical peer to assess. Simplicity belongs to the examples and their limits; it does not imply a hierarchy between writer and reader.

## Begin with transformations and their representation

[Chapter 1: Overview and Basics](chapters/01_OVERVIEW_AND_BASICS.md) introduces analogy, metaphor, changes of viewpoint and dimensionality, abstraction, salience, inversion, and reversibility. The triangle, square, prism, and subway map keep the relationships visible. This is a teaching foundation, rather than an exhaustive inventory of primitive faculties.

[Chapter 2: Compound Transformations](chapters/02_WORKING_WITH_TRANSFORMATIONS.md) develops further operations through behavior labels, conditions, sequences, interventions, connections, roles, requirements, and challenges. It shows how several moves can serve one purpose and leads into the repository's tools. Some operations remain individually useful; their placement here does not make every one a compound.

[Chapter 3: Sentence-Thought Vectors and the Framework](chapters/03_SENTENCE_THOUGHT_VECTORS.md) carries forward the substantive introduction formerly used as the README. It makes ontology, dynamics, regime, and object or destination explicit, then places concept extraction and the broader toolset around that representation. Its historical context remains supporting explanation.

The opening chapters preserve the distinction between a model's learned capabilities and the particular arrangements an application supplies. Information may come from training, supplied context, external retrieval, or tools; consequences inferred from that information and proposed alternatives have their own status.

Operation names enter with cases that give them a concrete meaning. The detailed family map follows the second chapter, where it is available as reference without carrying the opening exposition. Each movement develops one issue, with the examples presented as shared objects of analysis.

## Build toward the repository's designs

Four separate tool chapters follow the sentence-thought introduction:

| Chapter | Central work |
|---|---|
| [4. The Ontological Prism](chapters/04_ONTOLOGICAL_PRISM.md) | Distinguish the identity class being examined from the domain lens used to examine it. |
| [5. The Dynamical Prism](chapters/05_DYNAMICAL_PRISM.md) | Decompose a behavior into processes and retain the dependencies between them. |
| [6. The Regime Field](chapters/06_REGIME_FIELD.md) | Identify which conditions change the meaning or applicability of those processes. |
| [7. The Prism Coupler](chapters/07_PRISM_COUPLER.md) | Bind the separate accounts to actors, roles, objects, resources, and conditions. |

The chapters reuse a small calculator/checker/reporter case. Each develops one tool through a concrete difficulty, its supporting transformations, the capability their combination adds, an applicable limit, and a bounded request. Reusing the case lets the new distinction carry the reader's attention. The ontological chapter explains how the existing KCE and CDP definitions contribute; it does not invent another registered module.

Four further chapters develop how an account can become reusable and how alternatives can be constructed and compared:

| Chapter | Central work |
|---|---|
| [8. KCE: Extracting a Reusable Concept](chapters/08_KEY_CONCEPT_EXTRACTION.md) | Recover a governing relation, retain its conditions, and specify it in another situation. |
| [9. The Cognitive Transformation Registry](chapters/09_COGNITIVE_TRANSFORM_REGISTRY.md) | Select movements that preserve the concern while changing the view or arrangement. |
| [10. The Exploration and Transform Engine](chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) | Develop alternatives with consequential differences, dependencies, and return paths. |
| [11. PSPP: Comparing Candidate Systems](chapters/11_PARALLEL_SYSTEM_COMPARISON.md) | Compare what those alternatives support and retain the grounds for selection, combination or deferral. |

KCE returns here after its introduction in Chapter 3 so the completed representation can show what a generalization must preserve. This is an explanatory reading order. The source architecture places provisional KCE extraction before domain selection and coupling; an application can revisit it as its account changes. The book does not prescribe a universal execution pipeline.

Chapters 9–11 share the archive's access-and-preservation problem. The same concerns remain available while the method changes from choosing a movement to developing arrangements and comparing them. A settled local point becomes the starting point for the next consequential question.

The following conceptual sequence connects these chapters to the remaining reader guides.

| Conceptual step | What the reader needs to understand | Repository examples |
|---|---|---|
| Represent a thought | Entities, processes, relationships, conditions, objects, and consequences. | [Sentence-thought vectors](chapters/03_SENTENCE_THOUGHT_VECTORS.md) and the [O/D/R/O reference](ODRO.md). |
| Extract and reuse a concept | Abstraction, governing relations, applicability, and specification in a new situation. | KCE and the [worked examples](WORKED_EXAMPLES.md). |
| Explore other possibilities | Domain lenses, process and regime distinctions, candidate representations, and useful transformations. | Prism, Coupler, CTR, ETE. |
| Work with several perspectives | Conflict generators, necessary dependencies, compatibility, and changed arrangements. | CREM. |
| Compose a useful application | Candidate comparison, ordered dependencies, selective orchestration, and process oversight. | PSPP, CEC, DARE/IDCM and combinations appropriate to a particular design. |

Each module enters after the reader understands the problem it helps organize. The [module index](MODULES.md) supplies the detailed reference route. A reader may choose an existing arrangement, alter it, or design another one.

## Expository construction

Organize each section around a consequential distinction. Present the case, explain its governing relationship, and develop the consequence directly. Questions belong where an issue remains open; exposition carries relations whose outcomes can already be stated. Simple analogical cases retain boundaries visible inside the same example: an outline leaves part of a solid unseen, a connection map supplies no distance, and sorting cannot recover a discarded number. Preserve the intermediate explanation while reducing the number of premises. The nonfiction multiplex supplies candidate narration and attention constructions for this movement; it contributes no theory of model operation and does not establish the effectiveness of the resulting chapter.

The prose serves illustration, communication, and edification. Ordinary idiom and useful ambiguity can remain when they help carry the intended relationship; additional precision should earn the attention it consumes. Clarify a distinction where the example depends on it without turning each illustration into a specification.

The main prose explains. Compact tables support comparisons; diagrams can show relationships; examples connect abstractions to understandable situations. Detailed schemas, packet formats, the full transformation registry, and historical documents belong in reference material reached when needed.

Variation among models belongs within the explanation of capability. Naming an operation, carrying it out, and sustaining it across a complex task can make different demands. This practical qualification informs a designer's choices without becoming the book's central subject. Experimental protocols and model comparisons stay in [evaluation and limitations](EVALUATION.md).

The original [framework snapshot](../framework/), [provenance](PROVENANCE.md), and source manifest retain their existing roles. This editorial design changes the explanatory route. Chapters 1–11 provide the current reading route; the other individual guides remain starting pages for further development.
