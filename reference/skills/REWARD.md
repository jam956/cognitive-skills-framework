# Reward Controller: keep feedback separate from the solver's objective

For the extended treatment, see [Chapter 17: Reward Controller: Adjusting Future Effort](../../docs/chapters/17_AUDITOR_FEEDBACK_CONTROL.md).

**Question:** How should observed results change future effort without letting the solver redefine success?

## The problem and the method

“Improve yourself” leaves unclear what may change and who judges improvement. A solver that supplies its own favorable evaluation can reinforce the appearance of success rather than better outcomes.

Reward Controller specifies bounded feedback owned by an auditor or outer loop. It names criteria such as task completion, truth, coherence and attunement, and proposes small changes to future planning, exploration or verification settings. Governing constraints remain controlling.

## Historical development

Recovered December 7, 2025 discussion describes RewardController as an evaluator within a broad-to-narrow search strategy. The discussion explicitly distinguishes adaptive search/control from reinforcement-learning training.

A March 22, 2026 discussion considered combining it with the programming orchestrator at runtime while keeping the conceptual specifications separate. The cognitive-tools copy enters the surviving Git history on May 4. Its current contract restricts output to advisory future-assignment adjustments.

These are different integration contexts, not evidence that one automatic learning service operated across them all.

## Example and boundary

Repeated failures caused by omitted dependency checks might justify more verification effort on similar future work. The result must be grounded in actual failures, and the adjustment must remain within the host's authority.

The stored weights, caps and divergence inputs are configuration proposals. This repository neither measures all of them nor changes model weights. Claims of calibrated reward, automatic learning or a measured persona divergence require separate instrumentation and evidence.

**Read:** [Reward Controller specification](../../framework/RewardController_ParallaxEngine.v1.json) · [probe profiles](PROBES.md) · [DARE/IDCM](DARE.md) · [evidence trail](../../archive/HISTORY.md#evidence-trail)
