# Repo separation build loop

*Case 2 `02-repo-separation-build-loop` — presentation layer rehomed from the original pack reader. The [archived case JSON](case.json) and the raw records it references are authoritative.*

## Governance situation

An architectural boundary was turned into executable work, kept aligned across actors, and later corrected when the repository state diverged from the narrative.

The governance situation is a common failure point: a boundary decision sounds right, implementation begins, and the narrative can drift away from the repo. Here the decision is decomposed into work that can be built and inspected. When later verification finds the narrative stale, the correction lands back on the same operational thread.

## Judgment evidenced

The evidence shows a healthier operating cadence: architecture is not allowed to float above execution, and execution is not allowed to silently rewrite strategy. The record preserves whether a decision became a working capability, and whether later evidence changed the decision basis.

## Operating pattern in the records

The record keeps decision, scaffold, implementation, vertical-slice proof, CLI inspection, and later ground-truth correction in one operational chain.

## Selected evidence spine

- **Time: 12:51 · Type: CML · Record: `CML-17` · State: active · Emitter: Seb**
  Seb opens the repo-separation thread to turn a boundary decision into executable structure. The mandate is not only to discuss architecture, but to prove the split through working scaffolding.
- **Time: 13:06 · Type: INT · Record: `INT-44` · State: fyi · Emitter: code-framework**
  code-framework records scaffold completion and names the architecture contract. This gives the later implementation work a stable boundary rather than a loose repo-cleanup brief.
- **Time: 14:01 · Type: INT · Record: `INT-45` · State: proposed · Emitter: codex-build**
  codex-build clears governance-core work to proceed alongside runtime work. The reading is operational: separate streams can move in parallel because their ownership lines are explicit.
- **Time: 14:04 · Type: ACT · Record: `ACT-20` · State: recorded · Emitter: code-framework**
  code-framework implements the governance core store against governance-owned types. This is the first concrete proof that the repo boundary is being carried into code.
- **Time: 20:33 · Type: INT · Record: `INT-47` · State: proposed · Emitter: codex-build**
  codex-build defines the first vertical slice. The record compresses the architecture into a testable path through governance, runtime, and inspection surfaces.
- **Time: 12:50 · Type: CML · Record: `CML-22` · State: draft · Emitter: Seb**
  Seb opens the first vertical-slice execution intent. The thread narrows the architecture work to a proof that can be built, pushed, and inspected.
- **Time: 12:08 · Type: ACT · Record: `ACT-27` · State: recorded · Emitter: code-framework**
  code-framework implements and pushes the governance-to-runtime fold-back slice, then records the tests. The action links architecture intent to a verified build artifact.
- **Time: 12:45 · Type: ACT · Record: `ACT-33` · State: recorded · Emitter: code-framework**
  code-framework implements the CLI-facing execute-and-inspect contract. This makes the slice observable from the outside rather than only internally coherent.
- **Time: 17:28 · Type: INT · Record: `INT-98` · State: proposed · Emitter: code-framework**
  code-framework later corrects the repo ground truth after local verification. The correction prevents a stale architecture claim from becoming the release story.

## Trust movement

CML-17 -> INT-47 -> CML-22 -> ACT-27 -> INT-98

## Governance evidence

This is execution discipline plus correction discipline. The record does not stop at architecture intent; it follows whether the intent produced working surfaces, then accepts later ground truth when the implementation story needs updating.

## Verification links

[Case JSON](case.json) · `CML-17.json`, `CML-22.json`
