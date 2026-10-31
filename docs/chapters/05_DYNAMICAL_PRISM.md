# The Dynamical Prism

“The checker verifies a total before the reporter publishes it.” The sentence gives us a recognizable function. It leaves open what the checker receives, what establishes agreement, and how its decision reaches the reporter.

The [Ontological Prism](04_ONTOLOGICAL_PRISM.md) helps identify the kinds of entities and relationships involved. The **Dynamical Prism** turns attention toward what those entities do. Its practical contribution is to make an activity inspectable without treating its familiar name as an explanation.

## 1. Open the behavior label

Consider the calculation workflow from Chapter 2. Record `R17`, version `v1`, contains the values `7` and `5`. The calculator proposes the total `12`. In this example, checking means obtaining the two values, recomputing their sum, comparing it with the proposed total, and returning a decision tied to that record and version. Publication requires an approving decision.

“Checking” is a **computed behavior label**: a compact description of the function produced by the arrangement. The label becomes useful when its supporting actions are available for examination. It does not supply those actions by itself.

This is **label decomposition** applied to a process. *Abstraction* separates the checking function from the particular component named “checker.” *Decomposition* opens the function into actions. *Concretization* supplies the values, comparison rule, record identity, and expected decision.

The combination exposes a distinction that the opening sentence hides. A checker may establish that `7 + 5 = 12` while failing to establish which record the result belongs to. If the reporter attaches that approval to `R18`, the arithmetic agreement survives while the workflow's claim fails. We can now ask which relationship needs repair instead of asking vaguely for “better checking.”

The description remains a stipulated account of the task. Whether a particular checker performs it requires evidence about that checker.

## 2. Name the processes within the function

The reduced Dynamical Core offers process verbs for describing this activity. A few are sufficient here:

| Process verb | Its work in this example |
|---|---|
| *Detect* | Receive the values, proposed total, and record/version identifiers. |
| *Interpret* | Determine what the arithmetic agreement means under the stated checking rule. |
| *Encode* | Form a decision that retains `R17`, `v1`, the checked total, and the result of the check. |
| *Signal* | Transmit that decision to the publication boundary. |
| *Gate* | Permit the result to pass only when the required decision applies to it. |

These verbs describe different contributions. Receiving a decision is not the same as interpreting it; interpreting it does not ensure that its record identity survives transmission. The reporter's publication is a further action, which the core can describe through *execute*: causing the specified change in the reporting system.

The arithmetic comparison remains an explicit task step. “Compare” is not a separately registered primitive in this reduced core. Describing its contribution through *interpret* does not erase the calculation or claim that one verb explains its implementation.

*Classification* relates the concrete steps to the vocabulary, while *decomposition* keeps the distinctions visible. This adds a common process description that can survive changes in component names. The source calls its entries primitive process verbs as a modeling choice; it does not establish that they are irreducible faculties inside a language model.

## 3. Preserve the dependency between actions

Suppose the calculator sends `12` directly to the reporter and separately sends the checking material to the checker. All the named processes may occur. The reporter may still publish before the approval arrives.

The missing relationship concerns order and passage:

> Calculator result → checker decision → publication gate → reporter

Here, *signal* carries a decision and *gate* makes passage conditional on it. A useful gate rule is more specific than “an approval exists”: the approval must concern the same record, version, and proposed total as the item awaiting publication. An approval for `R17/v1` supplies no approval for a pending `R17/v2`.

**Topological rewiring** places the decision on the publication path. *Sequencing* retains the dependency between decision and publication. *Comparison* relates the identifiers and total at the boundary; *concretization* states what must match. Together these moves turn a collection of activities into an account of how the checking result affects publication.

This is why a list of active operators is insufficient. The list can include *detect*, *interpret*, *signal*, and *gate* without showing what is gated or which signal controls passage. The connecting relationships carry part of the function.

The revised path expresses a requirement. A real application also needs to enforce it. A diagram with an approval arrow does not establish that the reporter lacks a route around the gate.

## 4. Carry the function across implementations

The checker in this workflow could be a program, a person using a calculator, or a model supplied with the values and the checking rule. The process description gives us a way to discuss these alternatives while retaining the intended function.

For each candidate, the same questions remain available. Can it obtain the values for `R17/v1`? What does it use to determine agreement? How does it represent the decision? What receives that decision, and what conditions its passage to publication?

This is a controlled use of *abstraction*. We set aside the implementation long enough to retain the information and dependency pattern. *Concretization* then binds that pattern to a proposed implementation. Their combination supports **functional transfer**: another arrangement can be considered for the role because its contributions can be related to what the role requires.

The comparison also reveals missing work. A person may correctly recompute `12` but send only “looks right.” A program may preserve the identifiers but receive values from the wrong version. Each supplies part of the function while leaving a consequential relationship unsupported.

Shared process verbs do not make the candidates equally reliable. Nor does naming the checker an “independent verifier” establish independence from the calculator's evidence or method. Those claims require further details. The prism helps locate what to examine; the familiar behavior label remains a conclusion about the bound arrangement.

## 5. Use the process description to ask a narrower question

We can now return to the opening sentence with a more useful account. The checker receives specified material, determines agreement, preserves the decision's identity, and signals it. A gate conditions publication on that decision. “Verification before publication” names the combined function.

*Decomposition* opened the label, *classification* supplied process verbs, and *sequencing* preserved their dependencies. *Abstraction* made the pattern transferable; *concretization* kept it accountable to `R17/v1`. The added capability is an explanation that can guide a change: a missing identity field calls for a different repair from a reporter that publishes before receiving any decision.

The operating conditions still matter. The same gate could control a disposable test report or an authorized final release. Receiving the same approval signal need not permit publication in both cases. The next chapter holds the processes steady and examines those conditions through the **Regime Field**.

A bounded model request can keep this inquiry small:

> Apply the Dynamical Prism to this stipulated workflow: `R17/v1` contains `7` and `5`; the calculator proposes `12`; the checker recomputes and compares; the reporter requires approval for the same record and version. Describe the information path using only the relevant registered process verbs. Keep the arithmetic comparison explicit. Explain what fails if the reporter receives only “approved,” and identify the smallest missing relationship. Treat the description as a proposed arrangement, not evidence of execution.

Reference: [Dynamical Core specification](../../framework/Dynamical_Prism_v1.2_ReducedCore.json) · [Dynamical Prism guide](../skills/DYNAMICAL.md)

[Previous: The Ontological Prism](04_ONTOLOGICAL_PRISM.md) · [Next: The Regime Field](06_REGIME_FIELD.md)
