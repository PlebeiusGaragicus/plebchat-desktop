# PlebChat Desktop

Desktop builds of [PlebChat](https://plebchat.me) — the nostr-native,
ecash-paid AI workspace. The desktop app is the same client as the web
app, plus what a browser can't do:

- **Local folders** — mount folders from your computer into a Synthesize
  project; the agent reads and writes your real files (with approval),
  and external edits show up live.
- **No CORS wall** — read any RSS feed or article directly, and use any
  OpenAI-compatible AI endpoint, no proxy or scraping key needed.

## Install

Grab the installer for your platform from the
[latest release](https://github.com/PlebeiusGaragicus/plebchat-desktop/releases/latest):

| Platform | File |
|---|---|
| macOS (Apple Silicon) | `PlebChat_x.y.z_aarch64.dmg` |
| macOS (Intel) | `PlebChat_x.y.z_x64.dmg` |
| Windows | `PlebChat_x.y.z_x64-setup.exe` |
| Linux | `.AppImage` / `.deb` / `.rpm` |

> **macOS note:** builds are not yet notarized. The first launch needs
> **right-click → Open** (once) to pass Gatekeeper.

The app updates itself: it checks this repo's latest release on launch
and hourly, and asks before installing.

## About this repo

This repo hosts **releases only** — PlebChat's source lives in a private
monorepo, and the desktop app is built from a tagged commit of it by the
[release workflow](.github/workflows/release.yml) here (public repo =
free build minutes; each release names the tag it was built from).
Issues and feedback are welcome, either here or in-app (the feedback
button reports straight to the developers over nostr).
