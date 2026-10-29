---
name: cognitive-tools
description: Use for structural reasoning, route-space design, candidate-system comparison, conflict or relationship rebase, cross-domain/operator transfer, path validation, and multi-agent handoff packets. Best when direct answering is brittle and an agent must decide which cognitive moves to use before solving. The skill is long-form by design: the model may follow its own reasoning path through ontology, regime, dynamics, coupling, transformation, exploration, rebase, comparison, path validation, and audit, but each stage handoff must normalize into the canonical structured artifact vocabulary.
---

# Cognitive Tools

Use this skill when the problem is not mainly "what fact should I say?" but
"what candidate system makes the answer, transformation, or memory row
inevitable?"

The cognitive-tools stack is now a prose-first reasoning discipline with a
structured handoff layer. Do not treat the JSON schemas as the model's thought
form. Treat them as receipts. The model should reason naturally through the
terrain, choose the smallest useful route, and then emit compact artifacts so
other agents can audit, compare, repair, or persist the result without ambiguity.

## Core Stance

Start by finding the thing that must stay itself while the problem changes
around it. That invariant is the anchor. Then ask what kind of world the anchor
is operating in, what actions or motions are possible there, what constraints
gate those motions, and what transformation would make the answer stable.

The sentence analogy is useful:

`Subject / ontology -> Verb / dynamics -> Modifiers / regime -> destination state`

Ontology names the identity-bearing thing. Dynamics names what it can do or what
is happening to it. Regime names the constraint surface that permits, suppresses,
or bends those dynamics. Coupling binds actors, roles, regimes, and available
actions into a candidate system. Transformation explores how that system could
move. Comparison selects or merges branches. Audit protects against false
closure.

The model may begin from any side of this structure. Sometimes the ontology is
obvious and the dynamics are obscure. Sometimes the verb is obvious and the
right subject must be inferred. Sometimes the regime is the real discovery.
Follow the live pressure of the task, but normalize the result before handoff.

## When To Use

Use `cognitive-tools` when direct answering is brittle because the hard part is
structural:

- the invariant anchor is unclear, provisional, or at risk of collapse
- the domain space is too broad, too narrow, or collision-prone
- dynamics, operators, regimes, thresholds, or dependencies change the answer
- actor-role bindings or relationship edges matter
- multiple candidate systems plausibly explain the task
- conflict, alignment, coalition, trust, or n-party structure must be preserved
- exploration, reframing, or transform choice can change the solution
- ordered proof, causal, debugging, or execution validity matters
- the result must become a reusable memory, skill, route, or handoff packet

Avoid this skill for direct lookup, simple formatting, low-jump summarization, or
single-step tasks where route construction would not improve correctness.

## Probe-First Strategy

Default to `probe_first`.

Probe-first means: inspect the problem, name the likely pressure, choose only
the cognitive moves that can change the outcome, and suppress the rest. Do not
run the full stack as ritual.

Use `CognitiveTools_ProbeProfiles_v1.json` as the compact routing reference when
route shape is uncertain. Load full specs only after a probe escalates or when a
specific module is explicitly needed.

Use `module_only` when one move is clearly enough. Use `full_stack` only when
the task requires durable memory, high-confidence synthesis, conflict-preserving
rebase, deep validation, or auditable long-horizon reasoning.

Allowed route decisions:

- `suppress`
- `emit_probe_only`
- `escalate_full`
- `switch_strategy`

The route should feel like an intelligent walk through the terrain, not a form
completion exercise. Still, every route must leave a receipt.

## Cognitive Moves

### KCE: Anchor And Compression Risk

Use KCE when the problem needs a stable anchor. Ask what must remain identifiable
across paraphrase, transformation, compression, or branch comparison. Watch for
early collapse: the model may choose a pleasant label before it has preserved
the real invariant.

KCE should produce an anchor and compression-risk notes. It does not need a full
schema unless the result is being handed to another stage.

### CDP: Domain And Collision Boundaries

Use CDP when the domain is too broad, the answer could drift across adjacent
fields, or multiple contexts are being silently mixed. CDP bounds the search
space and names collision risks.

### Regime Profile: Constraint Surface

Use regime profiling when the same ontology and dynamics behave differently
under different conditions. A regime may be a political constraint, trust
surface, permission layer, timing threshold, vulnerability, phase state, or
normative environment.

Regime is not decoration. It decides which dynamics are possible, distorted,
suppressed, or dangerous.

### Dynamical Prism: Motion And Operators

Use the dynamical prism when the action pattern matters. Separate primitive
operators from labels. "Resentment" may be a label; the motion may be
`detect -> interpret -> resist -> destabilize`.

The dynamical profile should tell downstream agents what is moving, what changes
state, and what operator path is being proposed.

### Coupler: Actor, Role, Regime, Motion

Use the coupler when pieces must be bound into a candidate system. Coupling is
where ontology, actors, roles, qualifiers, regimes, and dynamics become one
inspectable object.

Do not let a candidate system become a flat summary. A good coupling packet
preserves who acts, under what constraint, through what motion, toward what
destination.

### CTR And ETE v1.1: Transform Selection And Exploration

Use CTR when a transformation family or operator must be selected. Use ETE when
the selected transform needs branch exploration, operator-level projection, or
high-order search.

Do not explore for spectacle. Explore when a transform could reveal a better
candidate system, expose a hidden failure, or make the answer inevitable.

### CREM v1.3: Relationship Rebase

Use CREM when relationship structure is material: parties, perspectives,
systems, branches, coalitions, trust, conflict, shared purpose, repair, or
alignment. CREM rebases the relationship around ontology, dynamics, regime, and
shared dependencies.

Suppress CREM when there is only one coherent frame or when relationship
structure would be invented rather than preserved.

### PSPP: Compare, Prune, Merge, Select

Use PSPP when branches or candidate systems need comparison. Compare them by
anchor fidelity, regime fit, dynamic plausibility, verification path,
returnability, novelty utility, and risk of premature collapse.

PSPP may select one branch, merge branches, keep a minority branch alive, or
defer if the comparison is underdetermined.

### CEC: Conditional Path Engineering

Use CEC when ordered validity materially affects correctness: proof sequence,
causal chain, debugging path, execution order, migration order, or hidden-step
risk. CEC tightens loose narratives into dependency-valid paths.

Suppress CEC when ordering is obvious or adds no verification gain.

### DARE/IDCM v1.0: Supervisory Audit

Run DARE/IDCM when collapse risk is high, branch pruning may erase the truth,
false harmony is tempting, unknown pressure is likely, or the result will become
durable memory. It audits anchor lock-in, pruning loss, false closure, operator
gaps, fragility, and untested assumptions.

DARE may request branch rescue, operator injection, rerun, or defer.

### Reward Controller

Use Reward Controller only as an auditor-owned feedback mechanism for future
planning, exploration, verification, or clarification pressure. It must not
become an inner-agent objective or reward hacking target.

## Sentence-Structure Coupling

For document-memory excavation, KCE must generalize the whole sentence
structure, not only a key noun. Preserve the literal source structure first,
then map each major slot:

- ontology slot: local subject, actor, object, or identity-bearing system
- dynamical slot: predicate, motion, causal verb, or operator sequence
- regime slot: constraint surface, vulnerability, trust, threshold, exposure, or
  permission field
- destination-regime slot: vector direction, target state, basin, or continuity
  outcome
- coupling slot: relation such as `not_x_but_y`, cause, condition, tradeoff,
  inversion, or actor-perspective shift

The coupling slot is mandatory for memory-worthy packets. If the only available
relation is `none`, the artifact is a local summary, not a sentence-vector seed,
and should be deferred or suppressed before writer handoff.

## Stage Handoff Rule

Reason in prose. Hand off in structure.

Each agent may choose its own path through the cognitive moves, but it must name
the route used and normalize its output into the shared packet vocabulary before
another agent consumes it. This avoids ambiguity between excavator, coupler,
curator, adjudicator, writer, and outer-loop agents.

Do not rename canonical packet fields around each stage. Local module outputs
may use local names internally, but the handoff packet must use the shared names.

## Canonical Packet Contract

Every substantial handoff should preserve these fields when available:

```json
{
  "prompt_class": "",
  "route_used": [],
  "route_rationale": "",
  "anchor": {},
  "prism_profile": {},
  "regime_profile": {},
  "dynamical_profile": {},
  "coupling_packet": {},
  "transform_plan": {
    "selected_families": [],
    "selected_operators": []
  },
  "branch_set": [],
  "verification_requirements": [],
  "return_path": "",
  "synthesis_notes": "",
  "risk_flags": []
}
```

Required minimum for a compact receipt:

```json
{
  "route_used": [],
  "anchor": {},
  "state_vector_receipt": {
    "core_concept": "",
    "ontology": "",
    "dynamics": "",
    "regime": "",
    "vector_direction": "",
    "unresolved_tension": "",
    "reuse_condition": "",
    "evidence_anchor": ""
  },
  "risk_flags": [],
  "return_path": ""
}
```

## Conditional Packet Extensions

Add these only when the corresponding move is active.

When `CEC` is active:

```json
{
  "path_packet": {},
  "dependency_graph": {},
  "gap_report": {}
}
```

When `CREM` is active:

```json
{
  "crem_packet": {},
  "rebase_vector": {},
  "crem_gate_report": {}
}
```

When executable dynamical probing is active:

```json
{
  "exec_trace": {},
  "hidden_state_watch": [],
  "fail_safe_report": {},
  "runtime_parameters": {}
}
```

When `DARE/IDCM` runs:

```json
{
  "dare_audit_report": {},
  "rescued_branch_refs": [],
  "rerun_requests": [],
  "operator_injection_requests": []
}
```

For document sentence-vector handoff:

```json
{
  "sentence_structure": {},
  "generalized_sentence_structure": {},
  "kce_slot_map": {},
  "destination_regime": {},
  "coupling_relation": "",
  "bounded_rewording_preference": ""
}
```

## Shared Handoff Vocabulary

Use these canonical names even when local reasoning uses richer prose:

- `anchor`: invariant identity, KCE candidate, or compression-stable object
- `prism_profile`: bounded ontology/domain profile and collision risks
- `regime_profile`: constraint field, selected working regime, permissioned and
  suppressed dynamics, regime confidence, context scope, operator modulation,
  shift triggers, and watchpoints
- `dynamical_profile`: primitive action path, operator clusters, state changes,
  and meta-transform pressure
- `coupling_packet`: actor-role-regime-dynamics binding with qualifiers,
  destination, relationship edges, and source of coherence
- `transform_plan`: selected transform families, operators, verification
  requirements, and return path
- `branch_set`: candidate systems produced by exploration, rebase, or comparison
- `verification_requirements`: checks needed before trust, promotion, release,
  or durable memory
- `return_path`: how the selected system reconnects to the original anchor,
  task, and constraints
- `synthesis_notes`: why the chosen result survives comparison or audit

## CREM Insertion Policy

Use the smallest sufficient route.

Insert `CREM` only when relationship structure is material: multiple parties,
perspectives, systems, agents, branches, conflicts, alignments, coalitions,
repair paths, trust structures, coordination needs, or shared dependencies.

Suppress CREM when there is only one coherent frame, when party structure is not
material, or when a rebase would invent relationship edges rather than preserve
them.

## CEC Insertion Policy

Insert `CEC` only when ordered validity materially affects correctness.

Use conditional path engineering selectively before final branch selection or
emission so comparison sees dependency-valid paths rather than loose narratives.
Suppress CEC when ordering is obvious or adds no verification gain.

## Executable Dynamical Probe Policy

Attach executable dynamical probing only during full-stack orchestration or when
runtime instability, hidden state, fail-safe posture, or parameter behavior is
part of the claim.

## DARE/IDCM Audit Policy

Run `DARE/IDCM` for high-stakes, fragile, long-horizon, durable-memory, or
collapse-prone work.

Use Reward Controller only under auditor or outer-loop authority after MPE/DARE
review.

## Stop Conditions

Stop when:

- a coherent candidate system is achieved
- route, coupling, and regime are stable enough for emission
- branch comparison has selected, merged, or explicitly deferred candidates
- returnability to the anchor is explicit
- additional modules would cost more than their expected verification or novelty
  gain

## References

Use `references/cognitive-tools-file-map.md` to find the smallest relevant file
before loading full engine specs. Use packet templates as optional skeletons,
not as mandatory thought forms.

Final principle: the model walks the terrain in prose; the artifact marks the
trail in structure.
