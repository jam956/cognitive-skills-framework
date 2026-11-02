# Cognitive Skills Framework

This book is a reference for software developers and AI engineers who want to make deliberate use of a language model's cognitive transformations. It develops the relationships behind analogy, abstraction, changes of viewpoint, concept reuse and the examination of alternatives, then shows how selected transformations can be organized into useful methods.

A model may work with information learned during training, supplied in a prompt or obtained from external sources. The further work concerns what it can do with that information: recognize a shared relation, identify a missing condition, construct another possibility or trace what a conclusion requires. The examples make those operations available for inspection and discussion. Their usefulness depends on preserving the facts, qualifications and relationships that matter to the task.

The repository's modules provide concrete designs to study and adapt. Each addresses a particular difficulty, such as an abstraction that loses its conditions, an exploration that repeats the same proposal, or a coherent answer that conceals a missing dependency. A designer can use a method directly, combine selected contributions or develop another arrangement for the application. The reading order supplies conceptual prerequisites; a particular task determines which methods it needs.

The book begins with simple examples and develops their logical progression before introducing the fuller tool designs. It also distinguishes a proposed explanation from supporting evidence, a procedure from its execution, and a useful result from a reusable method. Models differ in how reliably they perform these transformations, especially as the task becomes more complex.

## The book

| Chapter | Starting page | What it develops |
|---|---|---|
| 1 | [Overview and Basics](docs/chapters/01_OVERVIEW_AND_BASICS.md) | Analogy, metaphor, viewpoint, abstraction, salience, inversion, and reversibility. |
| 2 | [Compound Transformations](docs/chapters/02_WORKING_WITH_TRANSFORMATIONS.md) | Contributing moves, their combinations, and the capability each arrangement adds. |
| 3 | [Sentence-Thought Vectors and the Framework](docs/chapters/03_SENTENCE_THOUGHT_VECTORS.md) | Decompose a thought while preserving the relationships between its parts. |
| 4 | [The Ontological Prism](docs/chapters/04_ONTOLOGICAL_PRISM.md) | Identify what is being considered and select domain lenses that change the analysis. |
| 5 | [The Dynamical Prism](docs/chapters/05_DYNAMICAL_PRISM.md) | Open a behavior label into processes and dependencies. |
| 6 | [The Regime Field](docs/chapters/06_REGIME_FIELD.md) | Retain conditions that change meaning, permission, and applicability. |
| 7 | [The Prism Coupler](docs/chapters/07_PRISM_COUPLER.md) | Bind actors, roles, processes, objects, and conditions into a candidate system. |
| 8 | [KCE: Extracting a Reusable Concept](docs/chapters/08_KEY_CONCEPT_EXTRACTION.md) | Preserve a governing relationship while changing its level of generality and applying it elsewhere. |
| 9 | [The Circle and the Tilt](docs/chapters/09_THE_CIRCLE_AND_THE_TILT.md) | Keep a question in view while exploring supporting, opposing and reframed relationships. |
| 10 | [The Exploration and Transform Engine](docs/chapters/10_EXPLORATION_TRANSFORM_ENGINE.md) | Develop materially different candidate arrangements and retain their dependencies. |
| 11 | [PSPP: Comparing Candidate Systems](docs/chapters/11_PARALLEL_SYSTEM_COMPARISON.md) | Compare alternatives, direct consequential checks, and justify a choice or an unresolved result. |
| 12 | [CREM: Reframing Relationships](docs/chapters/12_RELATIONSHIP_REBASE.md) | Preserve distinct concerns and dependencies while changing a relationship. |
| 13 | [CEC: From a Proposal to a Valid Path](docs/chapters/13_CAUSAL_ENTAILMENT_CHAINING.md) | Expose consequential order, intermediate steps and missing dependencies. |
| 14 | [DARE/IDCM: Reopening the Frame](docs/chapters/14_DISCONTINUOUS_ANCHOR_RECONSTITUTION.md) | Audit assumptions, pruning and missing operations; reopen a route with retained constraints. |
| 15 | [Choosing and Combining the Tools](docs/chapters/15_SELECTIVE_TOOL_ROUTING.md) | Select the smallest useful operation, escalation level and receiving contract. |
| 16 | [Organ Atlas: Observing the Application](docs/chapters/16_OBSERVATION_AND_RECOVERY.md) | Relate qualified observations and proposed probes to recovery conditions. |
| 17 | [Reward Controller: Adjusting Future Effort](docs/chapters/17_AUDITOR_FEEDBACK_CONTROL.md) | Use auditor-owned, bounded feedback to guide future assignments. |
| 18 | [Open Questions and Further Directions](docs/chapters/18_OPEN_QUESTIONS_AND_FURTHER_DIRECTIONS.md) | Develop the unresolved design questions behind explanation, method preservation, expression and discovery. |
| 19 | [From a Useful Transformation to a Reusable Method](docs/chapters/19_FROM_TRANSFORMATION_TO_REUSABLE_METHOD.md) | Draw together what a method must retain so another practitioner can inspect, find and adapt it. |

Chapters 1–7 develop transformations and the O/D/R/O representation: ontology, dynamics, regime, and object or destination. Chapters 8–14 examine concept reuse, exploration, comparison, relationship rebase, ordered validity and process audit. Chapters 15–17 turn to selective application and optional observation and feedback. Each chapter can also be consulted for its particular question.

Chapter 18 develops the further design questions. Chapter 19 draws the common requirements together around what a useful transformation must preserve when it becomes a reusable method.

[Appendix A: Structured Handoffs and Packet Examples](docs/appendices/A_STRUCTURED_HANDOFFS.md) follows the archive case through seven packet templates and their shared index. The [module and file index in Appendix A](docs/appendices/A_STRUCTURED_HANDOFFS.md#module-and-file-index) connects every source definition to its chapter and contract. These routes account for all 23 JSON definitions and templates in the preserved framework.

## Appendices

[Appendix B: Applying and Assessing a Method](docs/appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md) combines the O/D/R/O reference, worked applications, and evidence and evaluation notes. It provides one route from representing a case to assessing what a use of the method establishes.

Appendix A also supplies the source-file index and handoff vocabulary. [Source and version notes](docs/appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#6-source-and-version-notes) follow the application material in Appendix B. The [source manifest](SOURCE_MANIFEST.json) records file identities and publication changes; historical and editorial records remain in the archive.

Published under the [MIT License](LICENSE).
