# The Prism Coupler

The preceding chapters separated the subject, processes, and operating conditions so each could be examined. The Coupler brings those accounts together and checks whether they describe one compatible arrangement.

## 1. A check bound to a different version

“The checker verifies a total before the reporter publishes it.” The sentence gives us a useful starting arrangement: a calculator produces the total, a checker examines it, and a reporter publishes the result.

For record `R17`, suppose the supplied facts are these:

- The checker approved the total in version 1.
- The calculator subsequently produced version 2, which the reporter now holds.
- Publication requires approval of the version being published.

All three components are present. Calculation, checking, and reporting are available, and a check occurred before publication. Nevertheless, version 1's approval does not authorize version 2. The second total could be correct; its correctness has not been established by that approval.

The missing relationship is between the check and its particular object. Connecting a checker to a reporter is insufficient if the reporter cannot distinguish which result was checked.

The **Prism Coupler** makes such relationships explicit. It binds actors, roles, operations, and operating conditions into a candidate account of a system. Its question is: **who or what does what, to which object, under which conditions?** Having the capabilities somewhere in a system does not establish that they are bound appropriately for the intended task.

## 2. Keep the fields distinct while joining them

The Coupler brings together the distinctions developed by the Ontological Prism, Dynamical Prism, and Regime Field. Each contributes something different to the calculation example.

Ontology identifies the kinds of things involved: programs, calculation records, and approval records. Roles describe their participation: the calculator supplies a proposed result, the checker examines it, and the reporter carries it into a published report. An actor can be a program, interface, or other structure with a consequential role; it need not be a person.

Dynamics describe the processes. The reduced operator vocabulary can distinguish execution, detection, and gating. In the proposed arrangement, the checker detects disagreement through the specified comparison, and the reporter gates publication according to version-specific approval. “Checking” is a human-readable behavior label supported by these actions and conditions. Treating that label as a primitive would conceal the work it summarizes.

Regime describes the conditions governing the work. The publication rule applies to the particular version being reported. The inputs and result are resources the checking role depends on. A proposed checker must be able to inspect them; assigning it a role does not supply that access.

A compact binding for the proposed arrangement could read:

| Actor | Bound work | Consequential dependency |
|---|---|---|
| Calculator | Produce a result from specified inputs. | Identify the input and result version. |
| Checker | Recompute the total and compare it with the proposed result. | Inspect those same inputs and that result. |
| Reporter | Publish an approved result. | Receive an approval referring to that result version. |

The table is a proposed contract. Whether the actual components exchange these records remains a separate question requiring inspection. A relationship edge in an account of a system needs evidence just as an individual capability does.

## 3. How the supporting transformations contribute

Several familiar transformations cooperate in this method. Their contributions become clearer when followed through the version mismatch.

*Abstraction* first isolates the governing relationship: approval applies to the object examined. The particular numbers can be set aside while this dependence is preserved. This makes the issue recognizable beyond arithmetic, wherever a check authorizes a particular item.

*Decomposition* then separates a compressed claim such as “the result was checked.” Which result was presented? What did the checker inspect? What did the approval refer to? What does the reporter hold? Separating these questions exposes the point at which version identity was lost. Merely listing the three components would leave that point hidden.

*Recombination* proposes a different arrangement of the resulting parts. The approval travels with a reference to the examined result, and publication depends on a match between that reference and the result being reported. Calculation and checking retain their functions; their products are joined more precisely.

*Concretization* supplies the particulars needed to inspect this proposal. In the example, the approval refers to version 1 and the reporter holds version 2, so the match fails. In an application, the designer must choose how records identify their versions and what changes produce a new version. The abstract relationship cannot choose or implement that mechanism.

*Evaluation* tests whether the binding preserves the requirement. If version 2 is checked and approved, it becomes eligible for publication under the stipulated rule. If the inputs subsequently change and a third version is produced, the earlier approval still cannot authorize it. That countercase tests the relationship rather than the mere presence of an approval record.

Together, these moves add an account of compatibility and dependence. We can explain why one arrangement meets the stated requirement and another leaves a gap. The Coupler organizes this work while preserving the separate fields needed to examine the explanation.

## 4. Begin with an actor or with an operation

An important strength of coupling is that the inquiry can start at either end of a relationship.

Starting with a known actor, we can ask which operations and roles its established capabilities support. Given a component that can inspect the current inputs and compare totals, checking is a candidate role. Its ability to check does not by itself establish authority to publish. Each additional binding requires its own support.

Starting with a desired operation, we can instead ask what could carry it. If the task requires checking the current total, a compatible actor needs the relevant data and the ability to perform the required comparison. The search can consider existing components or a proposed new component without assuming that either already meets those conditions.

If no carrier is established, the account should retain “checker candidate unknown.” The desired operation identifies a requirement; it does not conjure an actor, grant access, or prove independence from the original calculation. Likewise, two plausible carriers can remain alternate bindings when the supplied facts do not select between them.

This freedom makes the Coupler useful in design as well as diagnosis. A known component can suggest compatible work, and required work can guide a search for compatible components.

## 5. A bounded request and its limits

A model request can keep the attention on one unresolved binding:

> Apply the Prism Coupler to the calculator, checker, and reporter. Version 1 was approved; the reporter holds version 2; publication requires approval of the published version. Identify the actor–role–operation bindings and the version dependency. Distinguish supplied facts from proposed connections. Leave data access unknown where it is unspecified. Propose the smallest revised binding that preserves the rule, then examine what happens if the inputs change after approval.

The method can guide a prompt at this level or be supplied as an explicit structured contract. Neither use automatically implements a version check or guarantees that a model will preserve every dependency. The returned arrangement needs comparison with the actual application.

The Coupler specification also supports selective routing when a further kind of work is needed. For example, uncertainty about an ordered causal path can warrant **CEC**, while several materially different candidate arrangements can warrant comparison through **PSPP**. These are choices driven by the unresolved problem, rather than a requirement to invoke every module.

The central limit remains evidential. A coherent candidate system can describe how checking should govern reporting while the deployed reporter still accepts any total. Coupling helps make that difference inspectable. It establishes what must be connected and what remains unknown; verification must establish whether those connections actually hold.

Reference: [Prism Coupler v1.5 specification](../../framework/Prism_Coupler_v1.5_OntologyDynamicsRegime.json).

[Previous: The Regime Field](06_REGIME_FIELD.md) · [Next: KCE: Extracting a Reusable Concept](08_KEY_CONCEPT_EXTRACTION.md)
