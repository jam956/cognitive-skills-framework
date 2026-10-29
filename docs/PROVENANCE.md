# Source and version notes

## Publication source

The `framework/` directory is a complete, byte-preserved snapshot of `skills/cognitive-tools` from the `bounded-route-hyperagent` project at commit `dc6b7e536aeace455637fa22ce08edbbade712c4`.

It contains 28 files: one agent-facing skill guide, 23 JSON specification/template files and four reference documents, including a historical CREM PDF. The [manifest](../SOURCE_MANIFEST.json) records each file's size and SHA-256 hash. No personal memory databases, literary corpora, credentials or machine configuration files are part of this snapshot.

The public README and `docs/` guides are publication material accompanying that snapshot. They distinguish design intent from demonstrated behavior and explain the methods in reader-facing language. The snapshot's internal filenames, versions and module names are preserved.

## Why this copy

The project copy includes prose-first guidance and sentence-structure coupling additions. An older shared installation differed in three files: `SKILL.md`, `KCE_Parallax_v2.3_PacketTemplate.json` and `references/cognitive-tools-architecture.md`. This release uses the project revision consistently; it does not combine the two copies or change an installed skill.

## Reading the source specifications

- KCE's source module is named **Key Concept Extraction**; the evaluation uses **Key Concept Elevation** for the abstraction task. This publication retains both usages with their contexts.
- The Dynamical Prism's filename includes `v1.2`, while its internal reduced-core version is `v0.2.0_reduced_core`. Use the declared internal version when interpreting the model; the filename is retained for compatibility.
- Terms such as `design_stable_executable_spec` are historical design-status labels. They do not mean this repository includes an executable implementation or a validated cognitive instrument.
- Some source prose describes an answer as becoming “inevitable.” Read that as a design aspiration toward constrained, defensible selection, not a guarantee or a reason to discard uncertainty.
- The historical CREM PDF and the module's JSON specification reflect different stages of development. For the current documented split of ontology, dynamics and regime, use the v1.3 JSON and the skill guide.
- Retired filenames are listed for migration context. They are not missing current components.

## External companions

The specifications mention related components such as MPE, PSPE, ECE, an arbiter, memory curators, runtime monitors and provider-specific instrumentation. These are external interfaces or historical companion designs. Their mention does not imply that an implementation is bundled or that it runs when the documents are read.

## Updating this publication

Keep original snapshot changes distinct from explanatory edits. A future source refresh should name its revision, preserve provenance, update hashes and document any compatibility changes. A newly proposed algorithm belongs in the research notes until its contract and implementation status are explicit.
