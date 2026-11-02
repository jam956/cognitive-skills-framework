# The Regime Field

The checker has approved `12` for record `R17`, version `v1`, whose values are `7` and `5`. Its decision reaches a gate before the reporter can publish. We have described the information path. We still need to know where publication is allowed, which evidence the decision covers, and how long it remains applicable.

The **Regime Field** gives these operating conditions an explicit place in the account. It asks which conditions change the meaning or fit of the process we have described. The useful field is selective: a few consequential conditions can tell us more than an exhaustive set of loosely assigned categories.

## 1. Change the mode while retaining the actions

Suppose the workflow has two defined modes. In test mode, the reporter may write an approved total to a disposable preview. In release mode, it may publish the approved total to the final report only when a separate release authorization is present. These are rules stipulated for this example.

In both modes, the checker receives the calculation, determines agreement, encodes its decision, and signals the gate. The reporter then attempts to publish. The process verbs remain the same while the condition governing final publication changes.

This is **regime comparison**. *Abstraction* isolates the mode from the checking actions. *Comparison* holds those actions steady and examines what the changed permission allows. *Concretization* supplies the two destinations and the release requirement.

The combination lets us distinguish arithmetic approval from permission to release. Under the defined rules, “approved” can be sufficient for the preview while insufficient for the final report. Treating every approval as release authorization would silently transfer a condition from one mode into another.

The labels “test” and “release” have no such force by themselves. Their usefulness comes from the rules attached to them. Merely renaming a mode does not alter the gate's requirements or establish that the application observes them.

## 2. Keep possibility separate from permission

Now hold release mode fixed. Suppose the reporter has a working connection to the final report, but the separate release authorization has not been supplied. The transport is available; the gate must still withhold passage under the stipulated rule. A connection and permission to use it are different conditions.

Access and permission qualify different relationships. Access concerns whether the reporter can reach the destination. Permission concerns whether the governing conditions allow the action. A third condition may concern evidence: whether the checker can obtain the values needed to perform its assigned comparison.

*Decomposition* separates these conditions. *Comparison* prevents one from substituting for another. This adds a more useful diagnosis than “publication is blocked.” The reporter might need a connection, an authorization, or a completed check; those are different gaps.

The fuller Regime Field supplies axes such as `boundary_condition` and `authority_gradient`. They can help organize questions about passage and the distribution of permission. A compact profile can retain the concrete statement “final publication requires release authorization” alongside selected categories. The statement supplies the actual rule for this example.

A category does not establish who has authority. Nor does a writable destination confer permission merely because an action can succeed there. The model needs the stated rule or qualified evidence about it. If the authorization is unknown, the appropriate result is an unresolved permission condition, with its scope retained.

## 3. Bind the condition to the evidence it qualifies

Return to the approved total. The check concerns `R17/v1`. Suppose a revised version, `R17/v2`, is now awaiting publication. Leave the release authorization and all other conditions unchanged. Does the earlier approval cover the revision?

The arithmetic claim about `v1` remains intact. Its application to `v2` has not been established. Even if the proposed total is again `12`, agreement in the displayed number does not establish that the same input values were checked.

**Scope preservation** retains the relationship between a decision and its evidence. *Decomposition* separates the checked claim from the item now awaiting publication. *Comparison* examines their record and version references. *Concretization* identifies the evidence that would close the gap: the values and checking decision applicable to `v2`.

This lets the model preserve a supported result while limiting its reach. It can say “`v1` passed the arithmetic check; the check status of `v2` is unknown” without treating the revision as either approved or incorrect.

The compact **Regime Profile** provides places for context scope, active constraints, and evidence. Those fields make the qualification passable between stages. They do not supply the missing version or turn uncertainty into failure. The exact version condition can remain explicit even when no predefined regime category captures it neatly.

## 4. Let timing change applicability

Hold the record and version fixed again. Suppose the release authorization for `R17/v1` is valid until noon, and the reporter attempts publication at 12:05. The arithmetic check is unchanged; the permission condition has changed with time.

This is a **regime transition** within the same workflow. *Sequencing* locates approval, expiry, and attempted publication. *Comparison* relates the attempted action to the validity interval. The added capability is to recognize that a condition which held at the check may no longer hold when the result is used.

The profile's regime-shift triggers can preserve this transition: expiry calls for reconsidering publication permission. A broad tempo category alone would not carry the noon boundary. The exact interval belongs in the constraint account.

Suppose instead that the attempted publication time is unavailable. The result is a typed gap—unknown action time relative to the authorization interval. It is not evidence that publication occurred before expiry, and it does not establish that the checker failed its arithmetic task.

Changing one condition at a time has kept the consequences traceable. Changing the mode, version, authorization, and timing together would leave a much less informative explanation of why the action's status changed.

## 5. Preserve the scope of a negative condition

“The reporter is not permitted to publish `R17/v1` after noon” qualifies a particular action under a particular timing condition. It does not say that the total is wrong, that the checker withheld arithmetic approval, or that the reporter cannot publish a preview under the test rules.

*Decomposition* identifies what the negation governs. *Comparison* checks the proposed restatement against that scope. This supports **qualification preservation**: a compact handoff can remain short without changing the assertion it carries.

For this workflow, a useful handoff might retain release mode, the `R17/v1` evidence reference, the authorization interval, and any unknown attempted-publication time. The process description remains available beside it. Selecting these conditions is enough to answer the present question; the full field need not be populated.

The Regime Field therefore adds an applicability account to the Dynamical Prism's process account. Conditions remain provisional where the evidence is incomplete. The **Prism Coupler**, developed next, binds those accounts to the actors and roles that carry them.

A bounded request can focus the model on one change:

> Apply the Regime Field to the stipulated checker workflow. `R17/v1` contains `7` and `5`, and its proposed total `12` has passed the arithmetic check. Final release requires separate authorization valid until noon. Compare attempted publication at 11:55 and at 12:05, holding every other fact fixed. Identify the changed condition and its effect on permission. Preserve the arithmetic result and the scope of the negative conclusion. Then state the gap if the attempted-publication time is unknown.

Reference: [Regime Field specification](../../framework/Regime_Field_v0.1.json) · [compact Regime Profile](../../framework/CognitiveTools_RegimeProfile_v1.json) · [Regime guide](../../reference/skills/REGIME.md)

[Previous: The Dynamical Prism](05_DYNAMICAL_PRISM.md) · [Next: The Prism Coupler](07_PRISM_COUPLER.md)
