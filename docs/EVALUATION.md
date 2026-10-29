# Evaluation and limits

The framework is an explicit method collection. Its documentation, implementation in another project, successful use on one task and general effectiveness are different kinds of evidence.

## Existing evaluation

The [Key Concept Generalization and Specification Evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) includes:

- Encoding exercises: passage to governing concept, O/D/R/O and limits.
- A decoding exercise: a supplied Kissinger analytical framework and fictional facts to a new article.
- Separate dimensions for overgeneralization, undergeneralization, fidelity, structural transfer, writing quality and control-material leakage.
- An example report comparing Sol 6.1 at low reasoning effort with Qwen 3.8 27B, Q4_K_M, with thinking disabled.

The article task receives a prepared framework; it does not consume the model's preceding extraction. The example report contains six encoding cases and one article case per model, with separate, identity-masked AI review. Its judgments are provisional and have not been human-calibrated. Different backends and settings are recorded. This is evidence about particular outputs, not a broad model ranking or validation of every framework module.

## What a stronger comparison would require

Use comparable task inputs and settings across ordinary instructions and structured-framework conditions. Define the scoring criteria before examining outputs. Keep all attempts, failures and uncertainty; use reviewers who do not know the tested condition where practical. Evaluate new cases, including cases where the method should be suppressed.

Check whether any improvement is due to the framework's structure, the additional task information or simply a larger context budget. Measure costs as well as output quality. Repeated trials and independent human review matter before making general claims.

## Instrumentation boundaries

The JSON source specifications contain conceptual scores, thresholds, telemetry fields and runtime-probe proposals. This documentation release does not supply the instruments required to measure latent instability, neural attention, divergence, reward or every named confidence signal. A model-generated number is not automatically such a measurement.

Likewise, a schema-valid packet establishes only a structural property. Its source claims, applicability and proposed actions still require independent checks. Do not convert agreement between model roles into independent evidence of truth.
