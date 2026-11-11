---
name: thorian-connection
description: Connect or reconnect the Thorian beta plugin in Codex or a compatible host, or resolve missing tools and authentication errors. Use for plugin setup, not ordinary research.
---

# Connect Thorian beta

This package includes the tested thorian-skill 1.4.3 unchanged and a hosted MCP connection in Codex-compatible format. Use thorian-skill for research. These instructions handle plugin-managed setup; do not create a separate MCP registration.

Requires an approved Thorian account. Use the host's Connect or Reconnect control for this plugin. The service is https://beta.thorian.ai/mcp; the workspace is https://beta.thorian.ai. Installing this package grants no document access. Do not install another skill or MCP registration, remove an existing connection, or switch to another identity as a workaround.

In Codex CLI, inspect `codex mcp list` and `codex mcp get thorian` to confirm this plugin's server is loaded at https://beta.thorian.ai/mcp. Then `codex mcp login thorian` starts the packaged OAuth flow. This authenticates the bundled server; it does not create a standalone registration. Keep the command running while the user signs in. The registered return address is http://127.0.0.1:8769/callback/P0P5KSbj8csv; if that port is busy, let the other sign-in finish rather than killing an unrelated process or changing the callback.

Explain that the user signs in through the browser, completes authentication, reviews access, approves the requesting app through WorkOS and returns to the host. Passwords and authenticator codes stay in that flow, never chat. Use a fresh host-generated sign-in flow, not a bookmarked URL. A callback may be localhost or cloud-hosted; do not force a callback or alter client registrations.

After success, make one small read-only query through this plugin's Thorian tools. Only report a working connection after that call succeeds. If tools are missing, use a supported host refresh or explain that a fresh chat may be needed. Never substitute a local, legacy, synthetic or administrator connection. If the host cannot authenticate this portable plugin, report the limitation rather than inventing setup controls.

Authentication failures require reconnecting. Permission denials, capacity limits and service outages require their respective remedies, not repeated MFA. For unresolved problems, contact constantin@thorian.ai without sending tokens, passwords or private documents.
