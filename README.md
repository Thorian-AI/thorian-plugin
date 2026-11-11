# Thorian beta

Research your Thorian workspace from your agent, using graph relationships and cited source text.

This public repository distributes the beta plugin and research skill. **Using the service requires an approved Thorian account.** It is not a public OpenAI directory listing. Your documents stay in your permission-controlled Thorian workspace; this repository contains no documents, credentials or backend source code.

## Install in Codex

Use a current Codex version with plugin support. Add this marketplace and install Thorian:

```sh
codex plugin marketplace add Thorian-AI/thorian-plugin
codex plugin add thorian@thorian-beta
```

Open a fresh chat, select Thorian beta and ask:

> Connect Thorian beta, then use its research skill to summarize the key findings in one of my available documents, with source citations.

Use the host's connection/sign-in control when prompted. Sign in with your Thorian account, complete your authenticator check, review access and approve the connection. Enter passwords and codes only on the sign-in page. A localhost callback is normal for a desktop login.

The package includes the skill and remote MCP configuration; no local server, database or API key is needed. If you already have a standalone Thorian connection or skill, select this plugin explicitly to avoid ambiguity. Do not delete an existing connection just to try the plugin.

## Updates

```sh
codex plugin marketplace upgrade thorian-beta
codex plugin add thorian@thorian-beta
```

Open a fresh chat after updating. Release notes are in [CHANGELOG.md](CHANGELOG.md).

## ChatGPT

This repository is a portable package, not a universal ChatGPT installation link. Availability of repository/local plugins depends on the host and workspace. A custom MCP connection by itself does not install the bundled research skill. ChatGPT beta onboarding remains in [Thorian's Agents screen](https://beta.thorian.ai/ingestion#agents); do not assume an owner-only plugin link can be installed by another account.

## What is included

- Plugin `thorian`, version **0.1.0**.
- Research skill **1.4.3**, preserved byte-for-byte from the tested release.
- A plugin-specific connection helper and `https://beta.thorian.ai/mcp` configuration.

Research starts from graph relationships and uses original source text to resolve gaps or ambiguity. Extracted claims may be uncertain or incomplete; retain qualifications and check material findings against their cited sources. The integration provides read-only research access. The installed skill is readable by its users and is not a security control.

## Beta validation

Package validation and a clean Codex installation are checked separately from authenticated service access. Successful installation alone does not prove login works on every host. Each tester should complete sign-in and one small document query before relying on the connection.

## Help

Open your workspace at [beta.thorian.ai](https://beta.thorian.ai). For access or connection issues, contact **constantin@thorian.ai**. The skill itself does not expire; use the plugin's reconnect control if authentication expires. Please do not post private documents, passwords, tokens or authentication links in public issues.
