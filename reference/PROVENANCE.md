# Source and version notes

## Publication source

The `framework/` directory reproduces the complete `skills/cognitive-tools` package from the `bounded-route-hyperagent` project at commit `dc6b7e536aeace455637fa22ce08edbbade712c4`.

It contains 28 files: one agent-facing skill guide, 23 JSON specification/template files and four reference documents, including a historical CREM PDF. The [manifest](../SOURCE_MANIFEST.json) records each file's size and SHA-256 hash. All 23 JSON files and four reference documents remain byte-preserved. The skill guide has the front-matter repair recorded below; its instruction body is unchanged. No personal memory databases, literary corpora, credentials or machine configuration files are part of this snapshot.

The public README, book chapters, appendices and `reference/` guides are publication material accompanying that snapshot. They distinguish design intent from demonstrated behavior and explain the methods in reader-facing language. The snapshot's internal filenames, versions and module names are preserved.

## Skill guide publication repair

The source guide's unquoted YAML description contained `design: the model`. A YAML reader treated the colon as a mapping delimiter and rejected the front matter. The publication uses a folded scalar for that description; its wording and the full instruction body are unchanged.

The manifest records both the upstream and published size and SHA-256 identity for this one repair. The source revision remains the same. This is a metadata syntax correction, not a revision to the cognitive method or its JSON contracts.

## Why this copy

The project copy includes prose-first guidance and sentence-structure coupling additions. An older shared installation differed in three files: `SKILL.md`, `KCE_Parallax_v2.3_PacketTemplate.json` and `references/cognitive-tools-architecture.md`. This release uses the project revision consistently; it does not combine the two copies or change an installed skill.

## Reading the source specifications

- KCE's source module is named **Key Concept Extraction**; the evaluation uses **Key Concept Elevation** for the abstraction task. This publication retains both usages with their contexts.
- The Dynamical Prism's filename includes `v1.2`, while its internal reduced-core version is `v0.2.0_reduced_core`. Use the declared internal version when interpreting the model; the filename is retained for compatibility.
- Terms such as `design_stable_executable_spec` are historical design-status labels. They do not mean this repository includes an executable implementation or a validated cognitive instrument.
- Some source prose describes an answer as becoming “inevitable.” Read that as a design aspiration toward constrained, defensible selection, not a guarantee or a reason to discard uncertainty.
- The historical CREM PDF and the module's JSON specification reflect different stages of development. For the current documented split of ontology, dynamics and regime, use the v1.3 JSON and the skill guide.
- Retired filenames are listed for migration context. They are not missing current components.

## PSPP's numerical policy

The [PSPP v5.0-lite artifact](../framework/PSPP_v5.0_CandidateSystemComparator.json) is preserved as published. Its comparison method is clear, while two policy details need a consistent interpretation in an implementation:

- `lite_contract.dare_audit_surface` requires DARE review at pruning loss `>= 0.35` or fragility `>= 0.45`. The corresponding `operational_thresholds` are `0.45` and `0.55`. The file does not state a precedence rule or distinguish the two sets as separate stages.
- The minimal example reports a top-branch score margin of `0.05` and sets DARE audit to `recommended: false`, although the lite contract requires review below `0.08`. The example merges contributions for the Arbiter but does not explain an exemption from that trigger.

These are unresolved details within the source design. The chapter illustrates comparison and conditional selection without treating those numerical controls as calibrated measurements.

## External companions

The specifications mention related components such as MPE, PSPE, ECE, an arbiter, memory curators, runtime monitors and provider-specific instrumentation. These are external interfaces or historical companion designs. Their mention does not imply that an implementation is bundled or that it runs when the documents are read.

## Updating this publication

Keep original snapshot changes distinct from explanatory edits. A future source refresh should name its revision, preserve provenance, update hashes and document any compatibility changes. Prospective arrangements in [Chapter 18](../docs/chapters/18_OPEN_QUESTIONS_AND_FURTHER_DIRECTIONS.md) retain their open contract and implementation status. Development history is kept in the [archive](../archive/HISTORY.md), alongside the [editorial design](../archive/BOOK_DESIGN.md), outside the main reading route.
