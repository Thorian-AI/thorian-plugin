# Changelog

## 0.1.3

- Research skill 1.5.1 adds personal voices, document-assisted voice analysis and discovery for complex work or file outputs. Direct questions are answered without a discovery interview.
- Check the official release manifest on each skill invocation and load newer instructions for that task when available. Installed plugin updates still use the host's normal mechanism; caches and customized skills are not overwritten.
- Personal voices are accessible to the signed-in user's connected agents by default. Saving a voice requires user approval in the skill workflow. Document access remains read-only.
- Preserve the existing MCP URL, OAuth client, scopes and callback; no reauthorization is required solely for this update.

## 0.1.2

- Use the Codex-compatible manifest and MCP configuration so Codex 0.159.2 loads the registered OAuth client, read/refresh scopes and exact localhost callback.
- Keep research skill 1.4.3 unchanged. No account credentials are included.
- Supersedes 0.1.1, whose portable authentication extension is not loaded by this Codex version.
- Verified GitHub installation, browser sign-in and a read-only document query through the bundled MCP on Codex 0.159.2.

## 0.1.1

- Declare Thorian's registered public OAuth client and read/refresh scopes in the portable MCP configuration. No client secret is distributed.
- Superseded after authentication testing identified that Codex did not load this portable extension.

## 0.1.0

- Initial public repository distribution for the invite-only Thorian beta.
- Research skill 1.4.3 preserved unchanged.
- Portable hosted MCP configuration, plugin connection guidance and Codex marketplace installation.
- No OpenAI directory submission or backend deployment.
