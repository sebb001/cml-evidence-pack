# CML operational evidence pack

Coordination records from the lab where the Context Mediation Layer (CML)
was built and first used.

![Three framed prints: anaglyph glasses over blueprints — "So, this is 3D?"; a cat in an impossible box — "I was never there."; the cat wearing the glasses — "I'm right here, prove me wrong."](assets/ce-chat-la.png)
_An assortment of three states of epistemic certainty_

## What this is

One origin case and five later governance cases from a live CML instance.
The records show intents, interpretations, corrections, divergences,
authority-bound writes, and gated releases, with stable identifiers
throughout, so every claim in the briefs can be followed to a record.

Scope: this is n=1 self-evidence. The author was theorist, operator, and
primary evaluator. The pack shows the system in real use in one lab. It does
not show transferability to another team, and it is not an argument that
anyone should build on the companion repository rather than writing a fresh
implementation.

## Structure

- [`cases/`](cases/) — one directory per case, each holding a brief
  (`README.md`: situation, evidence spine, why it matters, record trail,
  records) and the case's record data (`case.json`: the context packets,
  with intents, interpretations, actions, reports, claims, and events
  grouped per CML intent).
- [`docs/`](docs/) — the [reading guide](docs/how-to-read-this-pack.md).
- [`00-tech-note.md`](00-tech-note.md) — how the records were produced, and
  the glossary.

The `case.json` files are the record layer and the authority for this
package. Briefs and docs are navigation. This is a lean dataset: it carries
the record structure the cases rest on, not the full lab substrate — see
Redactions below.

## The cases

| Case | What it shows |
| --- | --- |
| [Baseline recovery](cases/00-baseline-recovery-notion-prototype/) | The origin: recovering shared state after coordination collapse. |
| [Paperclip peer correction](cases/01-paperclip-peer-correction/) | An analysis peer-corrected and revised without hiding the original record. |
| [Repo separation build loop](cases/02-repo-separation-build-loop/) | A build decision carried through interpretation, action, and report custody. |
| [Substrate salvage](cases/03-substrate-salvage/) | A failing architecture direction superseded with provenance intact. |
| [Authority-bound write lane](cases/04-authority-bound-write-lane/) | Writes into shared state gated by explicit mandate. |
| [Gated release review](cases/05-gated-release-review/) | A release held at a review gate until the record supported it. |

## Naming

The records call the layer by its working name at the time, `3M-LAYER`. The
system is now published as the
[Context Mediation Layer](https://github.com/sebb001/context-mediation-layer).
The historical name stays in the records because it is part of the evidence.

## Redactions and integrity

This is a redacted, deliberately reduced public release: each case packet
contains only the records relevant to its case; personal and off-scope
records, the raw lab substrate, and the original delivery artefacts are not
included. Secrets, hostnames, client identifiers, and internal system names
are replaced with documented placeholders. [REDACTIONS.md](REDACTIONS.md)
records the policy. Within the published records, structure, identifiers,
and meaning are unchanged.

[MANIFEST.json](MANIFEST.json) records provenance and per-file hashes;
[SHA256SUMS.txt](SHA256SUMS.txt) covers the tree:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

## Related work

- [context-mediation-layer](https://github.com/sebb001/context-mediation-layer)
  — the runtime these records were produced with.
- [epilab](https://github.com/sebb001/epilab) — the simulation laboratory for
  the underlying governance primitives.
- [Governing Epistemic Systems](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6417898)
  (Bohle, 2026, SSRN) — the companion preprint.

## Licence

Copyright 2026 Sebastian Bohle. Licensed under
[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/):
read, share, and cite with attribution; no modified versions; no commercial
use. See [LICENSE.txt](LICENSE.txt).
