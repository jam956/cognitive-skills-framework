# Research notes and open questions

These notes separate prospective work from the preserved module specifications. They are proposals, not implemented features or established results.

## An explicit abductive loop

KCE can preserve alternative anchors; transformation and exploration can generate candidates; PSPP can compare them; DARE can challenge premature closure. An integrated abductive method would make the evidence relationships explicit:

1. Record the observation separately from its interpretation.
2. Propose rival explanations, including combinations or observation artifacts when warranted.
3. Derive consequences that distinguish the explanations.
4. Identify available evidence or a feasible check that could change their ranking.
5. Compare coverage, contradictions, regime fit and unsupported assumptions.
6. Retain a provisional explanation or suspend judgment, recording what would reopen the question.

The key addition is the link from an explanation to a discriminating prediction and then to evidence. Coherence alone is insufficient. The outcome field records what a hypothesis predicts, not what the investigator wants.

## Preserving a skill's shape

A reusable skill needs more than a name. A useful record could preserve purpose, applicability, transformation, invariants, destination, stopping conditions, examples and failure lessons. A separate experience record can link an execution to the skill version without silently rewriting the procedure after every use.

O/D/R/O may help qualify applicability; text supplies detailed instructions; an embedding may help find candidates. Their relative retrieval reliability requires evaluation. We should not infer a persistent learned procedure merely from a model's ability to reconstruct one from context.

## Attention and expression

The same analytical relation can be expressed in different voices and amounts of detail. How much of a writer's characteristic movement can a normalized representation preserve? Which features require examples, and which can be specified as relationships or sequencing constraints?

A related question is whether steering that improves sentence-level expression also preserves character independence, unresolved conflict and long-range causality. These should be evaluated separately.

## A library that remains discoverable

A method contributes only when a model or harness can find and apply it. Stable identifiers, applicability descriptions, versioned entry points and provenance may help bridge documentation, memory and runtime selection. Publishing this collection makes those interfaces inspectable; it does not itself provide a universal discovery service.
