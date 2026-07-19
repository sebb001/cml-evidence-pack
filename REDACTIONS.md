# Redactions

## v0.2 pass (private evaluation release)

Applied:

- Tailnet host suffixes and live public hostnames are replaced with placeholders.
- Local user paths are replaced with placeholders.
- Secret-file paths under service secret directories are reduced to redacted placeholders.
- Token-shaped strings, Bearer [redacted], private-key markers, GitHub token strings, and OpenAI-style secret strings are scanned before packaging.

Not applied:

- Stable CML, INT, ACT, RPT, and CLM identifiers are preserved.
- Actor names are preserved.
- Historical legacy product names inside record text are preserved where they are part of the evidence.
- Non-secret deployed file paths are preserved where they describe provenance or operational file-level changes.

## v0.3 pass (public release — lean dataset)

The public release is deliberately reduced relative to the private
deliverable:

- The raw lab substrate (full per-intent context packets, prototype-era
  vault and Notion source exports, architecture references) and the
  purpose-built HTML reader with its branding and audio artefacts are not
  included. The reader's glossary and per-case commentary are rehomed in
  the tech note and the case briefs.
- Each published case packet contains only the records relevant to its
  case. Records concerning the operator's personal work outside the cases
  (21 items across two packets) were removed rather than redacted.
- The client organisation's name and the name of the client contact are
  replaced with role descriptions ("the client", "a client executive").
- Internal lab system names and the actor names derived from them are
  replaced with consistent, role-preserving pseudonyms. The same original
  token always maps to the same placeholder, so cross-references remain
  intact.
- Network hosts, container identifiers, server filesystem paths, private
  workspace URLs, and one secret URL path are replaced with placeholders
  (`[redacted-host]`, `[container]`, `[server-path]`,
  `[notion-url-removed]`, `[redacted]`).
- The origin-case narrative was trimmed to a structural description of the
  coordination failure.
- Manifest and checksums were regenerated after all of the above.

Still not applied:

- Stable record identifiers, generic actor names, model/provider actor
  names, record structure, and record meaning are unchanged within the
  published records. Redactions replace or remove; they do not rewrite.
- The historical working name `3M-LAYER` is preserved inside record text as
  part of the evidence.

The full substrate remains in the private lab record and can be inspected
under agreement.
