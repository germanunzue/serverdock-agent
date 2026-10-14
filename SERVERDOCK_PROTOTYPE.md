# ServerDock Agent Prototype Boundary

This checkout is for internal development only until the feature's legal,
security, source-offer, signing and distribution gates have passed.

- Do not publish or distribute a ServerDock-branded Agent or viewer from this
  repository.
- Do not bundle a RustDesk-derived binary, library or asset into a ServerDock
  installer, `extraResources` payload or auto-update.
- ServerDock may launch a separately installed viewer with a non-secret Agent
  identifier only. Credentials, session content, remote input and frames remain
  inside the viewer and Agent boundary.
- Use only ServerDock-controlled rendezvous and relay infrastructure. Public
  RustDesk fallback and RustDesk WebSocket listeners are prohibited for the
  prototype.
- Keep each customization minimal, attributable and reviewable against the
  recorded upstream revision.

External distribution requires the evidence and approval described in
`specs/019-rustdesk-agent-access/` in the ServerDock repository.
