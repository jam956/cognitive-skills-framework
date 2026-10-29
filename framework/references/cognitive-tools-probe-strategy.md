# Cognitive Tools Probe Strategy

Use probe mode as the default entry to the cognitive-tools stack. Probe mode is
not a smaller copy of the engines; it is a routing and handoff filter that keeps
the stack cheap until a module can materially change the run.

Use `CognitiveTools_ProbeProfiles_v1.json` as the machine-readable contract for
the probe names, decisions, source specs, and stack presets below.

## Rule

Probe mode may classify, route, and emit compact handoff hints.

Full mode is required for:

- durable memory artifacts
- final high-confidence synthesis
- full state-vector or rebase-vector emission
- deep validation or proof claims
- branch selection that must be defensible
- supervisory audit that can mutate future agent, skill, or tool policy

Lite/probe modules should not be rewritten as full engines. They should be
tightened as audit-ready routing surfaces: each probe should say what it kept,
what it suppressed, why escalation was or was not justified, and which DARE/IDCM
watchpoints remain.

Each lite packet should preserve:

- `kept_fields`
- `suppressed_fields`
- `suppression_rationale`
- `escalation_rationale`
- `dare_watchpoints`
- `pruned_or_deferred_artifacts`
- `audit_stub`

The `audit_stub` is the compact reason DARE/IDCM can trust, challenge, or
request rerun of a lite decision.

## Probe Decisions

Each module probe returns one of:

- `suppress`
  Do not run the module.
- `emit_probe_only`
  Keep compact fields and continue.
- `escalate_full`
  Run the full module.
- `switch_strategy`
  Required inputs are missing or another route is better.

## Default Probe Order

Start with the structural substrate:

1. `KCE-probe::anchor_relevance`
2. `CDP-probe::domain_axis_fit`
3. `Regime-probe::constraint_surface_fit`
4. `Dynamical-probe::operator_cluster_fit`
5. `Coupler-probe::binding_fit`
6. `CTR-probe::transform_operator_need`

Then run the smallest conditional probe set:

- `ETE-probe::exploration_transform_value` when novelty, projection, or branch
  discovery may matter
- `CREM-probe::relationship_rebase_need` when conflict, alignment, repair,
  coalition, or n-party dependency structure may matter
- `PSPP-probe::branch_competition_need` when multiple candidate systems may
  compete
- `CEC-probe::path_validity_risk` when ordered dependency can change validity
- `DARE-probe::supervisory_audit_need` when the run is full-stack, fragile,
  high-stakes, long-horizon, or shows unknown-pressure

Do not run every conditional probe unless the outer loop is explicitly in
diagnostic or full-stack mode.

## Stack Presets

Use `direct_answer_probe_stack` when the task looks low-jump.

Use `state_space_probe_stack` when the task needs domain/operator/coupling
coordinates but not full branch competition.

Use `exploration_probe_stack` when transform execution, reframing, or
operator-level projection may create a better candidate system.

Use `candidate_system_probe_stack` when several systems could explain the task.

Use `relationship_rebase_probe_stack` when parties, perspectives, systems,
agents, or branches conflict or align around shared dependencies.

Use `verification_probe_stack` when proof, causal order, debugging, execution,
or hidden-step risk is material.

Use `supervisory_probe_stack` when DARE/IDCM should audit anchor lock-in,
pruning loss, false harmony, operator gaps, or fragile conclusions.

## Context Economy

Keep only:

- `anchor`
- `active_axes`
- `regime_id`
- `permissioned_dynamics`
- `suppressed_dynamics`
- `top_operator_clusters`
- `coupling_regime`
- `route_hint`
- `selected_transform_operators`
- `branch_need`
- `relationship_rebase_need`
- `verification_need`
- `supervisory_audit_need`
- `return_path`
- `basin_key`

Drop until full escalation:

- full traces
- exhaustive scores
- complete subdomain inventories
- all branches
- long prose rationales
- low-confidence edge cases
- every rejected branch unless DARE/IDCM is active

## Escalation Discipline

Escalate to a full module only when:

- the module can change route choice
- the module can change branch selection
- the module can prevent an invalid answer
- the module can produce or improve a durable memory artifact
- the module can preserve a return path that would otherwise be lost
- the module can detect fragility, false coherence, or unknown-pressure that
  should alter future policy

If none of those are true, keep the probe result or suppress the module.
