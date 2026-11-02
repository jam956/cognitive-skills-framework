# Organ Atlas: Observing the Application

An archive's document-delivery application has selected a reproduction for a wording request. During preparation, extraction fails on the same page several times. The application continues trying alternatives, but none establishes that the disputed passage is readable. The earlier access decision remains reasonable; the process carrying it out now needs attention.

What has the application observed, and what should happen before it sends a result? A retry record can establish repeated failures. It cannot establish the model's hidden instability or measure the entropy of its reasoning. That distinction matters when selecting both an instrument and a recovery action.

The **Organ Atlas** is an optional design scaffold for internal and latent-state probes, regulators, and fail-safe conditions associated with executable dynamical probing. The published template supplies names and proposed controls. An application must supply the instruments and implementation that would give those names operational meaning. We can inspect that design and consider how its separation of observation, interpretation, and recovery could guide a document-delivery application.

## 1. Start with the observation an instrument can support

Suppose a proposed delivery adapter records the page requested, the extraction attempt, the tool's returned status, and whether a usable result was produced. These records would support a narrow finding: three attempts returned errors for this page. They would not establish why the model continued, whether another method will succeed, or whether the source image is itself unreadable.

*Decomposition* separates the event from its explanation. *Classification* distinguishes a tool failure from a finding about the document. *Inference* then asks which explanations remain compatible with the record. Their combination prevents a recovery policy from answering the wrong problem.

An unavailable extraction service and an illegible reproduction need different responses. Retrying may serve the first if the service recovers. It cannot supply detail absent from the image. An inspection capable of assessing the marks is needed to distinguish those cases.

The adapter is a proposed application component, rather than a monitor included in the repository. Its event records would be evidence about visible execution. Any claim about latent properties would require a separately defined probe and an account of what that probe can establish.

## 2. Give each probe a functional question

The atlas names three monitored regions, called **tissues**: `reasoning_core`, `state_guard`, and `escape_router`. These are functional divisions in the template, not established anatomical regions or proof that an ordinary model API exposes corresponding internal components.

The reasoning core concerns multi-hop inference and plan chaining. Its proposed probes include operator-trace audit and stability comparison. The state guard concerns hidden instability, regime drift, and irreversible commitment risk; it names fail-safe flag audit, regime reclassification, and rollback readiness. The escape router concerns paradox pressure and fallback selection, including comparison of escape outcomes and confirmation of a fallback basin.

The useful question for a designer is what access each proposed probe would need. An operator-trace audit needs a trace whose meaning and coverage are defined. A rollback-readiness check needs an actual recoverable state. A model's explanation of its actions can assist review, but does not by itself expose the activations or causal processes behind those actions.

For the delivery application, an adapter might borrow the functional questions while retaining its own observable evidence:

| Functional concern | Proposed application-level check |
|---|---|
| Plan chaining | Do recorded attempts address the same missing evidence, or repeat a failed operation? |
| Commitment risk | Can the prepared response still be withheld or revised before dispatch? |
| Fallback selection | Does the alternative leave the unresolved passage explicit and preserve a route to review? |

*Abstraction* separates each function from its source-specific name. *Concretization* supplies an application check, and *comparison* identifies what that check actually covers. This adaptation does not turn the application's checks into the atlas's latent measurements. It makes the instrumentation gap visible enough to design around.

## 3. Keep the process description and the probe report distinct

The Dynamical Prism describes what a system does under particular conditions. Here, the application detects a failed extraction, interprets the result, explores another method, and eventually selects a response. Permissions and copy adequacy remain conditions on that process. Repeated exploration cannot authorize original handling or establish that the passage is legible.

The ordinary dynamical account is useful without runtime probes. When executable dynamical probing is active, the framework's skill guide additionally names `exec_trace`, `hidden_state_watch`, `fail_safe_report`, and `runtime_parameters`. The atlas provides the hidden-state watch and fail-safe report as an optional adjunct; it does not replace the dynamical profile.

These records have different jobs. An execution trace concerns what the implementation records as occurring. A hidden-state watch requires a qualified probing method. A fail-safe report concerns flags and recovery posture. Runtime parameters state the controls used. A field name alone supplies none of the observations needed to populate it.

The atlas makes this incompleteness explicit: its tissues have template status, and their entropy entries supply expected values while measured values remain null. The stored stability floors and entropy-divergence tolerances are design parameters. Before using them, an implementer would need to define the quantities, instruments, reference conditions, and evidence supporting a consequential threshold. Counting retries does not fill a missing entropy measurement.

## 4. Recover toward a state with fewer commitments

The delivery example has a practical recovery option. Keep the response as a draft, stop repeating the unsuccessful extraction route, and retain the passage as unresolved while an appropriate inspection is requested. A wording request still needs readable wording. The application can preserve that requirement without pretending to have met it.

This follows the atlas's proposed rollback posture: prefer a stable basin with lower commitment before further coupling or transformation escalation. In application terms, the recoverable state might be a held draft with its evidence attached. Once dispatched, the response may be correctable, but its earlier receipt cannot simply be undone.

The source's regulator priority names **interpret, select, stabilize, gate**. Applied to this proposed adapter, interpretation distinguishes the failure and its uncertainty; selection chooses a supported fallback; stabilization retains a coherent request and draft state; gating controls whether delivery proceeds. The implementation must enforce whichever dispatch boundary it promises.

*Phase decomposition* separates preparation from dispatch. *Counterfactual variation* asks what changes if another attempt also fails. *Evaluation* checks whether the fallback preserves the research requirement and permission boundary. Together they connect a flag to a meaningful action, rather than merely generating another warning.

The atlas also names irreversible-commitment guarding, rechecking coupling on instability, and surfacing hidden assumptions when flagged. Here the assumption worth exposing is that another extraction attempt will recover the needed detail. Recovery can return that assumption for inspection without claiming access to a hidden model state.

## 5. Invoke monitoring when it changes the next action

The atlas excludes direct tasks where a specification-level dynamical description suffices or a runtime probe would not change verification. An ordinary request to summarize a supplied, legible page may need neither a hidden-state watch nor a recovery subsystem.

The delivery case earns additional attention because an observed failure can affect dispatch. The designer still has to supply event capture, the relevant inspection, a recoverable draft state, and an enforced delivery gate. If internal-state probing is proposed, its access requirements and evidential limits belong in that design as well.

The combined capability is a traceable relation between an observation and a permitted recovery action. It allows the application to continue, pause, or return for evidence on stated grounds. Whether that improves the application requires implementation and testing.

> Review the proposed document-delivery process after repeated extraction errors on one requested page. Separate tool-return observations, interpretations, and unknowns. Identify which checks can use application records and which atlas probes would require unavailable internal instrumentation. Propose a recoverable state before dispatch and state what would permit resumption. Preserve copy adequacy and handling permissions as unresolved unless evidence supplies them. Use optional probe fields only where their method is defined; do not infer hidden-state entropy from retries or explanatory prose.

Reference: [Organ Atlas v0.3](../../framework/Organ_Atlas_Template_v0.3.json) · [Dynamical Prism](../../framework/Dynamical_Prism_v1.2_ReducedCore.json) · [conditional packet extensions](../../framework/SKILL.md#conditional-packet-extensions) · [instrumentation boundaries](../appendices/B_APPLYING_AND_ASSESSING_A_METHOD.md#5-instrumentation-boundaries).

[Previous: Choosing and Combining the Tools](15_SELECTIVE_TOOL_ROUTING.md) · [Next: Reward Controller: Adjusting Future Effort](17_AUDITOR_FEEDBACK_CONTROL.md)
