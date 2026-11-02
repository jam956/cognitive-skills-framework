# A Textbook for Designing with Cognitive Transformations

**Editorial design · reference edition, 1 November 2026**

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
| [9. The Circle and the Tilt](chapters/09_THE_CIRCLE_AND_THE_TILT.md) | Follow supporting and opposing views of a shared question, then introduce a distinction the opening frame could not express. |
| [10. The Exploration and Transform Engine](chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) | Develop alternatives with consequential differences, dependencies, and return paths. |
| [11. PSPP: Comparing Candidate Systems](chapters/11_PARALLEL_SYSTEM_COMPARISON.md) | Compare what those alternatives support and retain the grounds for selection, combination or deferral. |

KCE returns here after its introduction in Chapter 3 so the completed representation can show what a generalization must preserve. This is an explanatory reading order. The source architecture places provisional KCE extraction before domain selection and coupling; an application can revisit it as its account changes. The book does not prescribe a universal execution pipeline.

Chapters 9–11 share the archive's access-and-preservation problem. The circle and the tilt first make possible movements visible. ETE develops arrangements, and PSPP compares what those arrangements support. The CTR reference guide remains available for naming and selecting transformations. A settled local point becomes the starting point for the next consequential question.

Three further reasoning chapters develop the difficulties that a comparison can leave open:

| Chapter | Central work |
|---|---|
| [12. CREM: Reframing Relationships](chapters/12_RELATIONSHIP_REBASE.md) | Preserve coherent parties and shared dependencies while changing the structure of conflict or alignment. |
| [13. CEC: From a Proposal to a Valid Path](chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) | Test whether consequential intermediate steps and permissions support the route to a proposal. |
| [14. DARE/IDCM: Reopening the Frame](chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) | Inspect discarded alternatives, anchor choices and missing operations before authorizing a bounded correction. |

The archive remains a common case. The reader can follow how a relationship proposal acquires dependencies, how its ordered path is examined, and how an apparently sound selection can be reopened. Each chapter adds one governing issue while retaining the concerns established earlier.

The application section then examines how a designer can choose, observe and adjust a method:

| Chapter | Central work |
|---|---|
| [15. Choosing and Combining the Tools](chapters/15_SELECTIVE_TOOL_ROUTING.md) | Use Probe Profiles to select a sufficient operation, a compact result, fuller work or another strategy. |
| [16. Organ Atlas: Observing the Application](chapters/16_OBSERVATION_AND_RECOVERY.md) | Distinguish an actual observation from a proposed internal probe and relate qualified evidence to recovery. |
| [17. Reward Controller: Adjusting Future Effort](chapters/17_AUDITOR_FEEDBACK_CONTROL.md) | Keep evaluation with an auditor and apply bounded suggestions to future assignments. |

Chapters 16–17 are optional engineering references. Their proposed observation and feedback interfaces are explained through a document-delivery application without treating the source templates as installed instrumentation or model-weight training.

[Appendix A](appendices/A_STRUCTURED_HANDOFFS.md) develops selected-field packet examples and receiving-key translations. The seven templates and their index share that space, while modules with output definitions inside their main JSON link to the relevant contract. CTR remains a reference guide, following the book's chosen scope.

The unnumbered [afterword, From a Useful Transformation to a Reusable Method](AFTERWORD.md), provides the capstone. A document-lookup example develops what must survive when a useful correction becomes a method someone else can find and adapt. The prospective abductive loop illustrates a possible composition; method records, expression and discovery are examined through the same reusable-method question. Open contracts and unanswered application questions remain in the [research notebook](MUSINGS.md).

The following conceptual sequence summarizes the reading route.

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

The original [framework snapshot](../framework/), [provenance](PROVENANCE.md), and source manifest retain their existing roles. This editorial design changes the explanatory route. Chapters 1–17, the afterword and the handoff appendix provide the reading route. The shorter guides remain available for independent reference, with alternate examples and brief development notes. O/D/R/O is a compact glossary; worked examples support optional practice. History, evaluation and the research notebook remain supporting routes rather than additional prerequisite chapters. The module index and appendix connect every source JSON file to its explanatory use.
