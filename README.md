# rolfhelder's Claude Code plugins

[![CI](https://github.com/rolfhelder/claude-plugins/actions/workflows/ci.yml/badge.svg)](https://github.com/rolfhelder/claude-plugins/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

A Claude Code marketplace listing my plugins. Each plugin lives in its own repository, with its own README, changelog and issues.

## Install

```
/plugin marketplace add rolfhelder/claude-plugins
/plugin install keepalive@rolfhelder
/plugin install monitor@rolfhelder
```

From a shell, use `claude plugin marketplace add …` and `claude plugin install …`.

**Updates:** third-party marketplaces don't auto-update by default. Turn it on in `/plugin` → Marketplaces, or run `/plugin marketplace update rolfhelder`.

## Plugins

| Plugin | What it does | Platforms |
| --- | --- | --- |
| [keepalive](https://github.com/rolfhelder/claude-keepalive) | Keeps an idle session's prompt cache warm with one ping before it expires. Off by default. | any |
| [monitor](https://github.com/rolfhelder/claude-monitor) | RAM/CPU recorder with a live line in Claude Code and local logs for looking back at memory spikes. | macOS |

![keepalive and monitor above the prompt](https://raw.githubusercontent.com/rolfhelder/claude-monitor/main/assets/above-prompt.png)

## Issues

Report bugs and ideas in the plugin's own repository; each one has issue forms that ask for what's needed to reproduce.

## License

[MIT](LICENSE)
