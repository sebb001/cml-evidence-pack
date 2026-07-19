# CML operational evidence pack — technical note

Copyright 2026 Sebastian Bohle. Licensed under CC BY-NC-ND 4.0; see LICENSE.txt.

## What this is

This package contains one baseline recovery case from the Notion prototype instantiation and five raw Context Mediation Layer (CML) case packets from a live CML prototype instance (working name `3M-LAYER` at the time, preserved inside the records). The HTML reader provides orientation and navigation; the JSON records remain the source matter.

It also contains compact architecture references for orientation: the component slice map and governance schema source. Fuller architecture and contract doctrine are intentionally left for the repository review gate after the conversation.

## Origin context

The baseline recovery is a first-class origin case. Its prototype-era Notion source records are embedded in its case file; the standalone vault and Notion source exports are not part of this public release. This material has a different evidence standard from the five later cases: it is prototype-era source matter, not current resolver-backed JSON.

## How it was produced

The five later case records and the live origin anchors were retrieved from the live CML instance through neutral read access. The baseline recovery case uses prototype-era Notion and vault sources, added after checking that the full recovery packet was not present in the live resolver corpus. The earlier local HTML evidence pack was used only to preserve the later five-case selection and ordering. No role-bound MCP surface was used as the resolver for the CML records.

## Record glossary

- `CML`: Context Mediation Layer: the reference system that stores coordination records and their relationships.
- `intent (CML)`: The originating mandate, question, request, or operational scope.
- `interpretation (INT)`: An actor's reading of an intent or situation. Interpretations may align, diverge, ask for clarification, propose a path, or later be superseded.
- `action (ACT)`: An attributed record that work was performed against an intent, optionally linked to the interpretation that motivated it.
- `report (RPT)`: A structured status, evidence, decision, or review packet attached to an intent.
- `claim (CLM)`: An active or released assertion attached to an entity, usually used to make a temporary operating constraint explicit.
- `actor`: A registered human or agent participant that can author records, receive intents, and carry attribution.
- `role`: A named participation envelope with its own contract, policy, or context reference.
- `actor-role binding`: The registry link that allows a specific actor to operate through a specific role on a specific surface.
- `domain`: A concern area used to route, organise, and interpret work.
- `contract`: A versioned governance record that can be draft, active, superseded, or retired.
- `event`: A recorded lifecycle change for an entity, including actor, reason, snapshot, and timestamp where available.
- `status`: The lifecycle state of a record, such as draft, active, closed, proposed, flagged, superseded, retired, or recorded.
- `alignment`: The relation an interpretation declares to the matter it addresses: aligned, uncertain, divergent, or superseded.
- `supersession`: A replacement relation where a newer record takes over from an older one without deleting the old record.
- `scope`: The named operating area a record belongs to.

## Architecture references

The architecture references from the private deliverable are not part of this release; component and schema documentation lives in the runtime repository. Historical records may mention earlier publication assumptions; this public release is licensed under CC BY-NC-ND 4.0 (see LICENSE.txt), and the runtime is published separately under MIT.
