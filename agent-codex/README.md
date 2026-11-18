# Codex Agent

Chat with Codex through ACP. Install Node.js and the Codex CLI, then sign in with Codex. The first connection downloads the adapter.

```sh
fiveleaf plugin install agent-codex
```

Enable the plugin in **Settings → Plugins**.

If a previous connection stopped with `peer disconnected before response`, update the plugin with `fiveleaf plugin update agent-codex` and reconnect. If you registered Codex manually, update its adapter argument to `@agentclientprotocol/codex-acp@2.7.0`. An explicit `CODEX_PATH` selects the Codex executable.

Select **Codex** in the chat agent picker. FiveLeaf launches `npx -y @agentclientprotocol/codex-acp@2.7.0` using your local account configuration.

If npm reports `ENOENT` for its `_npx` cache, run the launch command in a terminal with a fresh npm cache, or install `@agentclientprotocol/codex-acp@2.7.0` globally and register `codex-acp` as a custom ACP command.
