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

### keepalive

When you stop typing, the prompt cache expires and your next message pays to rebuild it. keepalive sends one short ping just before that, only during your working hours. Off by default.

- `/keepalive` turns it on for this session, `/keepalive off` turns it off.
- `/keepalive setup 9 17 1-5` sets working hours and days; `/keepalive margin 5` sets how early the ping goes.
- `/keepalive view` moves the line between above the prompt and the status line.
- `/keepalive on --global` makes it the default for new sessions.




https://github.com/user-attachments/assets/f0f3f293-99a0-42ef-b906-fa9c927f2e97


Video tutorial (56 s). [Download the video](assets/keepalive-tutorial.mp4) if it doesn't play inline. Full docs: [claude-keepalive](https://github.com/rolfhelder/claude-keepalive).

### monitor

A small background agent samples RAM, cache, swap and CPU every five seconds. Claude Code shows a live line, and the logs stay on your Mac for fourteen days. macOS only.

- `/monitor` shows the live line.
- `/monitor view` moves it into the status line and back.
- `/monitor report 30m` finds the worst moment in a time window: peak RAM, peak CPU, the apps using the most memory, and pressure alerts.


https://github.com/user-attachments/assets/c3fa3844-85ee-490a-b7b7-f4001a704dd8




Video tutorial (57 s). [Download the video](assets/monitor-tutorial.mp4) if it doesn't play inline. Full docs: [claude-monitor](https://github.com/rolfhelder/claude-monitor).

## Issues

Report bugs and ideas in the plugin's own repository; each one has issue forms that ask for what's needed to reproduce.

## License

[MIT](LICENSE)
