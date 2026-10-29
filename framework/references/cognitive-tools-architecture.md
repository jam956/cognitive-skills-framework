# Cognitive Tools Architecture

This reference describes the current cognitive-tools stack after the latest
module reconciliation. It is operational, not theoretical: use it to decide
which files to load, which modules own each handoff, and where to suppress cost.

## Minimal execution order

0. Run the probe stack from `CognitiveTools_ProbeProfiles_v1.json` unless the
   caller explicitly requests a full module.
1. Score the prompt on ambiguity, novelty pressure, contradiction, constraint
   density, verification need, relationship structure, and supervisory risk.
2. Run `KCE v2.3` only if the anchor is not already explicit and uncontested;
   otherwise preserve the compact anchor candidate.
3. Run `CDP v1.2` only if domain selection, collision risk, or memory basin
   precision can change the route.
4. Emit `regime_profile` when operating conditions constrain which dynamics are
   legal, risky, permissioned, suppressed, or threshold-bound.
5. Run `Dynamical Prism` only if operator clusters, thresholds, or
   meta-transform pressure can change coupling or branch choice.
6. If full-stack orchestration needs runtime dynamical evidence, synthesize a
   reduced-core runtime probe packet from `Dynamical_Prism_v1.2_ReducedCore.json`
   with optional `Organ_Atlas_Template_v0.3.json` support and attach only
   `exec_trace`, `hidden_state_watch`, `fail_safe_report`, and
   `runtime_parameters`.
7. Run `Prism Coupler v1.5` to bind actors, roles, qualifiers, regimes,
   ontology, dynamics, and CREM-ready relationship edges.
8. Use `CTR v2.1` to select transform operators and verification requirements
   when route choice requires exploration or geometry change.
9. Run `ETE v1.1` when bounded exploration, operator-level projection, or
   branch discovery is needed.
10. Run `CREM v1.3` when conflict, alignment, relationship repair, coalition,
   or n-party dependencies need rebase before candidate-system comparison.
11. Run `PSPP v5.0-lite` to compare, prune, merge, or select candidate systems.
12. Run `CEC v1.1` only when ordered path validity is material.
13. Run `DARE/IDCM v1.0` as a parallel supervisory audit for full-stack,
    fragile, high-stakes, long-horizon, or unknown-pressure runs.
14. Run `Reward Controller` only as an auditor-owned bounded feedback layer
    after MPE/DARE review. It may emit dial nudges for future assignments, but
    it must not expose a scalar reward objective to inner agents.
15. Final arbiter synthesizes back to the anchor and emits only after
    returnability, coherence, verification posture, and unresolved tension are
    explicit.

## Probe-First Routing

Probe mode is the normal entry path for efficiency. It returns `suppress`,
`emit_probe_only`, `escalate_full`, or `switch_strategy` for each considered
module.

Use `emit_probe_only` when compact fields are enough for the next handoff. Use
`escalate_full` when a module can change route choice, branch selection,
verification outcome, durable memory artifact quality, or future policy. Use
`suppress` when the module would add cost without changing the decision. Use
`switch_strategy` when required inputs are missing or a different route is
better.

The machine-readable probe profiles live in
`../CognitiveTools_ProbeProfiles_v1.json`.

## Packet Templates

Packet templates are optional full-execution skeletons. Load
`CognitiveTools_PacketTemplateIndex_v1.json` first, then load only the template
for the module being fully executed. Templates should never replace the
canonical orchestration packet; they provide richer local structure that must be
normalized back into the shared handoff vocabulary.

## Lite Module Purpose

The current pipeline does not require lite modules to become full duplicate
engines. Lite/probe surfaces should remain cheap decision layers. Their job is
to classify, preserve compact handoff fields, expose escalation triggers, and
make suppression defensible.

DARE/IDCM changes how lite modules are supervised, not their core purpose. A
lite module should now emit enough decision artifact for DARE/IDCM to audit:
what was suppressed, what was pruned, why escalation was skipped, and which
operator gaps remain. Full modules still own deep execution.

Minimum lite audit fields are `kept_fields`, `suppressed_fields`,
`suppression_rationale`, `escalation_rationale`, `dare_watchpoints`,
`pruned_or_deferred_artifacts`, and `audit_stub`. PSPP-lite additionally emits a
`dare_audit_surface` with pruning loss, selection margin, fragility, operator
gap suspicion, verification gaps, rescue candidates, rerun requests, and
operator-injection requests.

## Route decision table

- `KCE_CDP_DYN_COUPLER_ARBITER`
  Use when direct system construction is likely sufficient.
- `KCE_CDP_DYN_COUPLER_CTR_ETE_ARBITER`
  Use when exploration, operator-level projection, or transform execution is
  needed.
- `KCE_CDP_DYN_COUPLER_CTR_ETE_PSPP_ARBITER`
  Use when multiple viable candidate systems compete.
- `KCE_CDP_DYN_COUPLER_CREM_PSPP_ARBITER`
  Use when coherent relationship/conflict/alignment frames share dependencies
  and need CREM before PSPP.
- `KCE_CDP_DYN_COUPLER_CTR_ETE_CREM_PSPP_ARBITER`
  Use only when exploration and relationship rebase are both justified.
- `KCE_CDP_DYN_COUPLER_PSPP_CEC_ARBITER`
  Use when branch comparison or final emission depends on ordered path validity.
- `KCE_CDP_DYN_COUPLER_CTR_ETE_PSPP_DARE_ARBITER`
  Use when a full-stack or fragile run needs supervisory audit before final
  emission.

Legacy labels containing `MPO` or `META` should be treated as compatibility
aliases for `CTR -> ETE -> Arbiter` unless a historical artifact must be read as
written.

## Responsibility boundaries

- `KCE` owns provisional anchors, compression telemetry, abstraction variants,
  transform seeds, and sentence-structure coupling across ontology,
  dynamical, regime, destination-regime, and coupling-relation slots.
- `CDP` owns domain axes, subdomains, energy allocation, breadth budgeting,
  domain collisions, and domain-lock risks.
- `Regime Profile` owns the lightweight constraint surface between ontology and
  dynamics: candidate regimes, selected working regime, context scope,
  constraint field, operator modulation, shift triggers, DARE watchpoints, and
  compact search aliases.
- `Dynamical Prism` owns primitive operator clusters, operator vectors,
  computed behavior-label policy, and meta-transform pressure.
- `Dynamical reduced-core probe` owns optional runtime dynamical probing.
- `Organ Atlas` owns optional hidden-state and fail-safe watch scaffolding.
- `Prism Coupler` owns actor-role-regime binding, relationship edge detection,
  binding stability, and post-Coupler route gate hints.
- `CTR` owns transform family/operator vocabulary, selection rules,
  verification requirements, and return-path requirements.
- `ETE` owns exploration execution, operator-level projection, branch discovery,
  projection ledger, high-order search, and rejected-branch artifacts.
- `CREM` owns n-party conflict/alignment/relationship rebase, dependency
  invariants, latent axes, relationship rebase plans, and rebase vectors.
- `PSPP-lite` owns candidate-system ingest, branch scoring, differential
  verification routing, pruning, merge/select decisions, and decision artifacts.
- `CEC` owns dependency unroll, missing-middle audit, path packet emission, and
  gap reports.
- `DARE/IDCM` owns supervisory audit, anchor suspicion, pruning-loss audit,
  false harmony detection, operator-gap requests, branch rescue, and bounded
  discontinuous reconstitution.
- `Reward Controller` owns bounded auditor-side dial nudges from truth, task,
  coherence, attunement, humility, safety, and KL/deception penalties. It does
  not own primary solving, route generation, or memory writes.
- `Final Arbiter` owns final answer posture and synthesis back to the anchor.

## CREM Conditions

Run `CREM` when:

- at least two coherent parties, perspectives, systems, agents, or branches are
  in tension or alignment
- shared dependencies are explicit or suspected
- the task involves repair, coalition, relationship strengthening, synthesis,
  strategy, interpretation, or novelty
- preserving the original relationship structure matters during reframing

Avoid `CREM` when the task is single-frame, simple fact retrieval, only semantic
conflict, or one party frame is incoherent and needs basic correction first.

## ETE Conditions

Run `ETE` when:

- direct construction is too narrow
- operator-level projection may create a better candidate system
- CTR selected transforms require execution rather than labels
- novelty pressure is material and returnability can be preserved
- candidate branches need discovery before PSPP can compare them

Avoid `ETE` when the direct branch is adequate, projection would be ornamental,
or the transform has no return path unless DARE explicitly authorizes bounded
discontinuity.

## CEC trigger conditions

Run `CEC` when the task requires:

- proof or derivation
- causal or mechanistic explanation
- state tracing or ordered execution
- debugging or dependency ordering
- missing-middle repair between anchor and conclusion
- branch comparison where sequencing affects validity

Avoid `CEC` when the answer is direct and low-jump, ordering is obvious, or
added path structure would not improve verification.

## DARE/IDCM trigger conditions

Run `DARE/IDCM` when:

- anchor lock-in is suspicious
- pruning has high information loss
- false harmony or forced alignment is possible
- a relationship-strengthening task risks party erasure or manipulation
- ETE rejected branches may contain a rescued candidate
- operator gaps or unknown-pressure remain after ordinary repair
- a long-horizon or outer-loop run may mutate future tools, skills, agents, or
  memory policy

DARE/IDCM is a supervisory counteragent, not the primary solver.

## Executable Dynamical Probe Conditions

Run the executable dynamical probe when:

- full-stack orchestration is active
- operator conflict, paradox pressure, or regime instability could change branch
  selection
- hidden-state uncertainty or fail-safe posture needs to be surfaced explicitly

Project parameters may adjust executable-probe thresholds through named
organ-atlas profiles or explicit overrides. These changes tune sensitivity and
fail-safe posture; they must not alter the canonical packet contract.

## Packet contract

Every stage handoff should preserve:

- `prompt_class`
- `anchor`
- `prism_profile`
- `regime_profile`
- `dynamical_profile`
- `coupling_packet`
- `route_choice`
- `transform_plan`
- `branch_set`
- `verification_requirements`
- `return_path`
- `synthesis_notes`

Add these only when `CEC` is active:

- `path_packet`
- `dependency_graph`
- `gap_report`

Add these only when `CREM` is active:

- `crem_packet`
- `rebase_vector`
- `crem_gate_report`

Add these only when executable dynamical probing is active:

- `exec_trace`
- `hidden_state_watch`
- `fail_safe_report`
- `runtime_parameters`

Add these only when `DARE/IDCM` is active:

- `dare_audit_report`
- `rescued_branch_refs`
- `rerun_requests`
- `operator_injection_requests`

## Shared vocabulary

Normalize local module outputs into the orchestration vocabulary before handoff:

- `anchor` <- `KCE.anchor_candidates`
- `prism_profile` <- `CDP.output_contract.prism_profile`
- `regime_profile` <- ontology/prism evidence, prompt operating conditions,
  dynamical operator pressure, and Coupler regime policy
- `dynamical_profile` <- `Dynamical Prism.output_contract.dynamical_profile`
- `coupling_packet` <- `Prism Coupler.output_contract.coupling_packet`;
  preserve `regime` and `regime_ref` for compatibility
- `transform_plan` <- `CTR.selected_transform_plan`
- `branch_set` <- `ETE.candidate_system_branches`,
  `CREM.candidate_system_branches`, or `PSPP.candidate_systems`
- `crem_packet` <- `CREM.crem_packet`
- `verification_requirements` <- route policy, CTR checks, PSPP differential
  verification, CEC gaps, CREM gates, or DARE audit requests
- `return_path` <- transform, rebase, branch-selection, or final arbiter logic

Keep these names stable at the cognitive-tools layer even if local module
schemas use different labels.

## Verification contract

Before final emission, confirm:

- invariant preserved or explicitly traded off
- prism breadth justified
- dynamical profile justified
- executable dynamical probe justified when used
- hidden-state watch and fail-safe report reviewed when produced
- coupling and regime are coherent
- transform use justified and returnable
- CREM preserved relationship dependencies when used
- PSPP branches are materially distinct
- dependency ordering justified when `CEC` is active
- DARE/IDCM audit reviewed when active
- unsupported jumps or inserted assumptions are explicit
- unresolved tension is stated if not fully resolved

## Failure rules

Do not:

- lock a single anchor when KCE marks it provisional
- activate broad prism coverage because it feels richer
- treat operator vectors as ontology by themselves
- keep coupled systems without actor support or regime coherence
- run ETE as ornamental metaphor
- run CREM as compromise-only conflict smoothing
- branch in PSPP without materially different systems
- keep transformed branches that cannot reconnect to the anchor
- emit ordered answers that skip prerequisite steps
- let DARE/IDCM become the primary solver

## Linked specs

- [CognitiveTools_ProbeProfiles_v1.json](../CognitiveTools_ProbeProfiles_v1.json)
- [CognitiveTools_PacketTemplateIndex_v1.json](../CognitiveTools_PacketTemplateIndex_v1.json)
- [cognitive-tools-probe-strategy.md](cognitive-tools-probe-strategy.md)
- [cognitive-tools-file-map.md](cognitive-tools-file-map.md)
- [KCE_Parallax_v2.3_SplitLayerAnchor.json](../KCE_Parallax_v2.3_SplitLayerAnchor.json)
- [CDP_Parallax_v1.2_BoundedDomainSpace.json](../CDP_Parallax_v1.2_BoundedDomainSpace.json)
- [Dynamical_Prism_v1.2_ReducedCore.json](../Dynamical_Prism_v1.2_ReducedCore.json)
- [Regime_Field_v0.1.json](../Regime_Field_v0.1.json)
- [Organ_Atlas_Template_v0.3.json](../Organ_Atlas_Template_v0.3.json)
- [Prism_Coupler_v1.5_OntologyDynamicsRegime.json](../Prism_Coupler_v1.5_OntologyDynamicsRegime.json)
- [CTR_Parallax_v2.1_SplitTransformRegistry.json](../CTR_Parallax_v2.1_SplitTransformRegistry.json)
- [ETE_v1.1_SplitLayerExplorationTransform.json](../ETE_v1.1_SplitLayerExplorationTransform.json)
- [CREM_v1.3_SplitOntologyDynamicsRegime.json](../CREM_v1.3_SplitOntologyDynamicsRegime.json)
- [PSPP_v5.0_CandidateSystemComparator.json](../PSPP_v5.0_CandidateSystemComparator.json)
- [CEC_Parallax_v1.1_ConditionalPathValidator.json](../CEC_Parallax_v1.1_ConditionalPathValidator.json)
- [DARE_IDCM_v1.0_ParallelSupervisoryLayer.json](../DARE_IDCM_v1.0_ParallelSupervisoryLayer.json)
