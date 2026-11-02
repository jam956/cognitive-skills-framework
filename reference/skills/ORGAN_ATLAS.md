# Organ Atlas: name the monitoring surface before claiming a measurement

For the extended treatment, see [Chapter 16: Organ Atlas: Observing the Application](../../docs/chapters/16_OBSERVATION_AND_RECOVERY.md).

**Question:** What observable signals, probes or recovery conditions would a deployment need?

## The problem and the method

A system can describe itself as unstable, coherent or improving without defining what was observed. The Organ Atlas is an optional scaffold for naming monitored regions, regulators, probe methods and fail-safe conditions.

Within the published package it supports the Dynamical Prism's optional runtime probes. It does not replace the ordinary dynamical description or require every task to perform monitoring.

## Historical development

Conversation-history retrieval finds the exact artifact name Organ_Atlas_Template_v0.3.json in an October 20, 2025 Prism v13 discussion, alongside control bundles and probe-handshake work. That establishes an early appearance of the atlas idea, not byte identity with the current file.

The current copy is present in the May 3, 2026 working baseline and supplies project-tunable thresholds, optional hidden-state watch fields and recovery posture. The exact revision path between the early artifact and this snapshot has not been fully recovered.

## Example and boundary

An instrumented application might observe repeated execution failures or resource exhaustion and use those signals to change its recovery policy. A model claiming an entropy gap without a defined instrument has not measured one.

Some atlas fields concern latent or internal properties unavailable through ordinary chat APIs. They remain proposed instrumentation interfaces unless a deployment supplies the required access and measurements. The documentation release contains the template, not that instrumentation.

**Read:** [Organ Atlas v0.3](../../framework/Organ_Atlas_Template_v0.3.json) · [Dynamical Prism](DYNAMICAL.md) · [evaluation boundaries](../../docs/appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#3-distinguish-illustration-from-evidence) · [evidence trail](../../archive/HISTORY.md#evidence-trail)
