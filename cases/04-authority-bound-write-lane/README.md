# Authority-bound write lane

The [case JSON](case.json) is authoritative; this brief is navigation.

## Situation

Agent access was treated as governance, not plumbing. Write capability was tested, separated from neutral access, and constrained through role, surface, and authority records.

The governance situation is the one every organisation will face as agents become operational: a useful agent needs access, but convenience can collapse roles, permissions, and accountability into a single bridge. Here the work starts with a scoped write test, then separates neutral MCP access from privileged advisory authority. The permission story is recorded as claims and actions rather than assumed from configuration.

Actions prove what the bridges allow; claims define authority boundaries; the record separates actors, roles, neutral access, privileged advisor authority, and deployed tool surfaces.

## Evidence spine

- **Time: 2026-04-26 19:42 · Type: CML · Record: `CML-34` · State: active · Emitter: codex-build**
  codex-build opens the reading-partner write-bridge thread. The question is whether a constrained agent lane can write to the vault without turning every connector into a general write surface.
- **Time: 2026-04-26 19:46 · Type: ACT · Record: `ACT-76` · State: recorded · Emitter: codex-build**
  codex-build deploys the scoped reading-partner MCP write bridge. The action establishes a limited write path whose authority is tied to a role and use case.
- **Time: 2026-04-26 20:09 · Type: ACT · Record: `ACT-78` · State: recorded · Emitter: reading-partner**
  reading-partner performs a permitted vault append through the scoped lane. This proves the lane can write, but only inside the policy envelope being tested.
- **Time: 2026-04-26 20:35 · Type: CML · Record: `CML-35` · State: active · Emitter: codex-build**
  codex-build opens the Principal Advisor topology thread. The matter shifts from a single scoped bridge to the broader question of who may use privileged advisory tools.
- **Time: 2026-04-26 20:37 · Type: ACT · Record: `ACT-83` · State: recorded · Emitter: codex-build**
  codex-build provisions the ChatGPT Principal Advisor route. The route is created as a specific authority surface rather than a generic MCP endpoint.
- **Time: unknown · Type: CLM · Record: `CLM-6` · State: active · Emitter: Seb**
  Seb constrains Principal Advisor authority to the ChatGPT app using GPT-5.5 high reasoning. The claim is an authority marker: it says which role exists, where it may operate, and which model posture anchors it.
- **Time: 2026-05-01 10:44 · Type: ACT · Record: `ACT-118` · State: recorded · Emitter: codex-build**
  codex-build separates neutral MCP access from the ChatGPT-only Principal Advisor role. This keeps general retrieval and role-bound authority from collapsing into the same surface.
- **Time: 2026-05-06 15:53 · Type: ACT · Record: `ACT-129` · State: recorded · Emitter: codex-build**
  codex-build enables the PA-bound 3M MCP vault write profile. The write capability is persisted as a named profile, not implied by ordinary read access.
- **Time: 2026-05-16 08:04 · Type: ACT · Record: `ACT-156` · State: recorded · Emitter: codex-build**
  codex-build exposes the current 3M MCP tool surface on the public ChatGPT bridge. The resulting bridge is broad enough to operate, while the authority story still depends on the role and scope records.

## Why it matters

This is authority design under agentic pressure. Access control becomes legible rather than asserted: instead of relying on a claim that agents are connected safely, the record exposes the authority topology. It decomposes access into who can act, under which role, through which surface, with which constraints, and with what proof that the lane works.

## Record trail

CML-34 smoke writes -> CML-35 role topology -> CLM-6 -> ACT-156

## Records

[Case JSON](case.json) — embeds the full context packets for `CML-35` and `CML-34`.
