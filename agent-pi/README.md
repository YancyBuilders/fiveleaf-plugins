# Pi Agent

Install Node.js 22 or later and Pi, then sign in and choose a provider in Pi. If FiveLeaf cannot find `pi`, set `PI_ACP_PI_COMMAND` to the absolute path of its executable. The first connection downloads the pinned adapter.

```sh
fiveleaf plugin install agent-pi
```

Enable the plugin in **Settings → Plugins**.

Select **Pi** in the chat agent picker. FiveLeaf launches `npx -y pi-acp@0.0.34` using your local account configuration.
