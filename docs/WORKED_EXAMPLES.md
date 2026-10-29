# Worked examples

These are original illustrative examples, not recorded model trials or scored results. They show observable task descriptions and concise decision artifacts. They are not transcripts of a model's private reasoning.

## 1. Extract a relationship without making it universal

**Source:** A repair team can diagnose a failed pump. Another organization alone can unlock the control cabinet required to repair it. No alternative access route is currently available.

**Method:** KCE, with the O/D/R/O distinctions.

**Candidate concept:** Technical competence does not remove dependence on a party that exclusively controls necessary access.

**Check:** The source supports diagnosis, not mastery of every repair. It does not establish refusal or hostile intent. A viable alternative access route would change this particular dependency.

Try supplying the source and method to a model, then inspect whether its concept preserves those qualifications. Compare against the same task without the method; keep all attempts.

## 2. Preserve disagreement while enabling action

**Situation:** Two groups share a maintenance system. One wants more control over upgrades; the other wants dependable shared operating standards. Both still need the maintenance system.

**Method:** Coupler and CREM, with comparison if several proposals remain viable.

**Candidate reframe:** Distinguish authority over an upgrade from responsibility for shared operating standards. Consider an arrangement that separates those decisions while retaining the shared maintenance dependency.

**Check:** The proposed distinction is a candidate, not an agreement already reached. Neither group's demand establishes that its preferred arrangement is feasible. Practical cooperation need not imply trust or resolution of the underlying dispute.

## 3. Guide an article's movement

**Task:** Write an analysis of a fictional infrastructure negotiation using only supplied facts.

**Contextual guidance:** Establish the shared objective; distinguish technical feasibility from approval authority; preserve the parties' different dependencies; develop a conditional proposal only after the diagnosis.

**Check:** Does the finished article follow the relevant relationships without inventing a withdrawal, a motive or a successful negotiation? Does it read as an article rather than as a list of control instructions?

The [KCE evaluation](https://github.com/jam956/Key_Concept_Generalization_and_Specification_Eval) supplies a concrete version of this experiment, including the Kissinger framework and a rubric. Consult its task files for exact model inputs and its separate review materials for scoring.

## A compact trial instruction

> Use the supplied facts as evidence. Identify the governing relationship and the conditions under which it applies. Apply only the cognitive method relevant to the task. Give the requested answer, followed by a short record of the method used, preserved constraints and unresolved uncertainty. Do not invent numerical measurements or imply that a proposed check has been performed.

This instruction is a starting point. The source specifications offer fuller stage and handoff definitions when a task requires them.
