# How to read this pack

## Authority order

1. `cases/*/case.json` — the record layer: context packets grouping
   intents, interpretations, actions, reports, claims, and events per CML
   intent. These are the evidence in this release.
2. `cases/*/README.md` — per-case briefs (situation, evidence spine, why it
   matters, record trail, records).
3. This documentation.

## Suggested route

- Read the [README](../README.md) for scope and claim boundaries.
- Read the six [case briefs](../cases/) in order. The origin case explains
  why the system exists; the five live cases each stand alone.
- For any case that earns your scepticism, open its `case.json` and follow
  the spine's record identifiers into the packet data.

## What the records are

Each context packet groups records around one CML intent. Record types and
lifecycle states are defined in the [tech note](../00-tech-note.md)
glossary. Stable identifiers (`CML-*`, `INT-*`, `ACT-*`, `RPT-*`, `CLM-*`)
are preserved, so a reference in a brief can be followed into the packet
data. Each brief ends with a Record trail: the case compressed to its
pivotal records, in causal order — the shortest path through the packet.

## Evidence standards

The five live cases are resolver-backed JSON (records retrieved from the
live system's read API rather than reconstructed by hand) obtained through
neutral read access. The origin case is prototype-era Notion source matter
embedded in its case file — a weaker evidence standard, included as a
first-class case because it documents why the system exists.

## Redactions

See [REDACTIONS.md](../REDACTIONS.md). This release is a lean dataset:
case packets contain only case-relevant records, and sensitive tokens are
replaced with placeholders. Within the published records, structure,
identifiers, and meaning are unchanged. The full lab substrate remains in
the private record and can be inspected under agreement.

## Integrity

```sh
shasum -a 256 -c SHA256SUMS.txt
```

`MANIFEST.json` records provenance and per-file hashes for the release.
