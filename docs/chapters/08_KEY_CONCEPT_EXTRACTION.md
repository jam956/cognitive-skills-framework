# KCE: Extracting a Reusable Concept

The checker approved version 1 of a calculation record. The reporter now holds version 2. Under the rule developed in the preceding chapters, approval must concern the version being published. The earlier check leaves the later version's status unresolved.

A software team encounters a similar difficulty. Its tests passed, but the artifact awaiting deployment was rebuilt afterward. The names and activities differ. What can be carried between these situations without treating them as the same event?

**KCE—Key Concept Extraction—** makes that question explicit. It identifies a governing relationship, considers a useful level of generality, and retains the conditions that make the relationship applicable. *Elevation* describes the movement toward a more general concept; *specification* brings that concept down into another case. Chapter 3 introduced this movement. We can now examine what the earlier prisms and Coupler help it preserve.

## 1. Recover the relationship behind the incident

“The reporter used the wrong version” describes the immediate problem. “Checking is important” offers a broader statement, but leaves the consequential relationship unstated. Neither yet explains what another designer could recognize in a different application.

In the calculation case, the decision concerns an examined item. A later item is presented for publication. The rule requires a check applicable to that later item, and the existing decision does not establish one.

One candidate concept is:

> When a decision rests on examining a particular item, applying that decision to a changed item requires support that the decision still applies to the changed item under the rule.

The numbers `7`, `5`, and `12` can disappear from this description. The connection between the decision and its evidence cannot. Removing the numbers changes the level of description; removing that connection changes the thought.

*Decomposition* separates the examined item, decision, later item, and publication requirement. *Relation extraction* recovers what connects them. *Abstraction* replaces their particular names with roles. Together these moves turn an incident into a relationship that can be recognized elsewhere.

The resulting statement is a candidate explanation. Its usefulness depends on whether it still accounts for the source case and what another situation requires.

## 2. Preserve what the familiar label leaves open

The word “approval” appears to carry the result on its own. Its meaning depends on what was approved and under which rule. In the earlier workflow, arithmetic agreement and permission to release were separate matters. A short concept can lose that distinction even while retaining the word.

Suppose the extracted statement becomes “approved work may be published.” It now joins a check to an action that the check may never have authorized. The compression has supplied a new relationship rather than preserving the old one.

The same problem appears in the software example. “Tests passed” needs an object and a scope: which artifact, which tests, and which relevant conditions? Whether that result is sufficient for release remains a further question. A familiar behavior label can conceal these different contributions.

KCE's split-layer description keeps provisional candidates for the entity, process, conditions, and participating roles. The Coupler can subsequently examine their binding. Naming a component “checker” supplies a useful role description while leaving its actual evidence and access to be established.

Here, *label decomposition* opens “approval” into the claim it carries. *Comparison* distinguishes that claim from permission to publish. Their combination preserves a qualification that a fluent summary could otherwise erase. It also gives us a concrete diagnostic question: what did the shorter statement add, omit, or change?

## 3. Find a useful level of generality

An abstraction can remain too close to the incident or move beyond what it supports. Consider three descriptions:

| Description | Logical fit and limits |
|---|---|
| R17 version 1 was checked; the reporter holds version 2. | Preserves the incident, with its reusable relation still implicit. |
| A decision based on one item needs a supported scope before it is applied to a changed item. | Retains the relation while allowing different objects and implementations. |
| Every change invalidates every earlier result. | Extends the claim beyond the evidence, resulting in overchecking. |

The third statement is decisive but excessive. The arithmetic result concerning version 1 remains valid. A change can also be irrelevant to the property being checked. Reusing evidence may be justified when the relevant object and conditions remain equivalent; that equivalence needs its own support.

The useful level therefore depends on what the concept is intended to carry. For version-specific publication, the item reference is consequential. For a collection of examples of sums equal to 12, record identity may contribute nothing to the task.

An **abstraction ladder** makes these alternatives available for inspection. *Concretization* returns each general statement to the source; *comparison* examines what it still explains. A countercase tests its boundary. The combination helps locate a portable statement without mistaking greater breadth for greater usefulness.

The specification calls for reporting compression loss. A concise note—“this version omits the separate release rule”—can be more informative than a confidence number. It identifies what a later application must recover.

## 4. Keep consequential alternative anchors available

Even a faithful description can foreground different relationships. The calculation example supports several possible anchors:

| Candidate anchor | Question it helps organize |
|---|---|
| Preserve the identity of the checked item. | Did the result become attached to another record or version? |
| Preserve the scope of the evidence. | Does the earlier check establish the property now being claimed? |
| Preserve the connection through the handoff. | Did the decision reach its recipient with enough information to apply it? |

These descriptions overlap, but they can lead to different repairs. A missing identifier calls for a different intervention from an inadequate test or from a decision stripped of its scope during transmission.

KCE retains alternatives when choosing one would conceal a consequential uncertainty. The current question gives a working anchor its purpose. A request to repair the report may foreground identity; a request to reuse an earlier check may foreground evidence scope. Later findings can change that choice.

This combines *salience reweighting* with *comparison*. The case remains available while one governing relationship becomes prominent. Holding a working anchor provisionally lets the inquiry proceed without making the first clear formulation control every subsequent step.

A small set is sufficient when its members expose the live alternatives. Rewording one anchor three times adds little; preserving three different possible failure locations can change what happens next.

## 5. Specify the concept in another situation

Return to the software team. Its passing test result concerns an earlier artifact; a later build is awaiting deployment. Applying the concept requires concrete counterparts:

| Calculation case | Software case |
|---|---|
| The examined record version | The tested artifact and relevant configuration |
| The checking decision | The result for the stated test set |
| The version held by the reporter | The artifact awaiting deployment |
| Approval applicable to the published version | Test evidence applicable to the artifact being considered |

*Analogy* proposes the correspondence. *Concretization* supplies the target objects and conditions. *Evaluation* asks whether the relationship survives. A matching word such as “version” is insufficient if the two applications use it differently.

The team can now ask whether the rebuild changed anything relevant to the tests. If that relationship is unknown, the concept has located a useful question. It has not established that the new build is defective or that every previous result must be discarded.

A reusable record can retain the source case, candidate concept, applicability conditions, and a countercase that limits it. Categories help retrieve the record; the preserved relationship helps assess its fit. KCE emits such candidates in the framework. A separate storage procedure decides whether and where they become durable records.

The contribution is a controlled movement from incident to concept and back to application. We can recognize the relation in another domain while keeping the evidence and qualifications that made it useful.

A bounded request can make that movement inspectable:

> Apply KCE to the version-checking example. Identify a reusable relationship and state what must survive when the record names and numbers are removed. Retain an alternative anchor if it would lead to a materially different repair. Give an overgeneralization and explain its failure. Then apply the supported concept to a rebuilt software artifact, leaving the relevance of any changes unresolved where the facts do not establish it.

The next chapter follows possible movements around a preserved question. The circle and the tilt give us a picture of changing a view or frame before the registry makes transformation choice explicit.

Reference: [KCE v2.3 specification](../../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) · [short KCE guide](../skills/KCE.md) · [O/D/R/O reference](../ODRO.md).

[Previous: The Prism Coupler](07_PRISM_COUPLER.md) · [Next: The Circle and the Tilt](09_THE_CIRCLE_AND_THE_TILT.md)
