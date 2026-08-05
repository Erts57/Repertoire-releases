# Repertoire

**Repertoire** is a desktop visual database builder. Design custom data models and explore them through tables, canvases, and other views — locally, offline-first.

This repository hosts **downloadable builds only** (installers, updater metadata, and license). It is not the application source tree.

## Download

Get the latest release:

**[→ Latest release](https://github.com/Erts57/Repertoire-releases/releases/latest)**

| Platform | What to download |
| -------- | ---------------- |
| **Windows** | NSIS installer (`.exe`) |
| **macOS** | `.dmg` (Apple Silicon builds from CI) |
| **Linux** | `.deb` or AppImage |

Exact asset names appear on each release page. Each release also includes `README.md` and `LICENSE` as downloadable assets next to the installers.

## Install notes

Installers are **not OS code-signed** yet. You may see SmartScreen (Windows) or Gatekeeper (macOS) warnings. That is expected until signing is enabled.

After install, the app can **auto-update** from this repository. Update packages are signed with Repertoire’s updater key (separate from OS code signing).

## What this repo contains

- GitHub Releases with platform installers
- Updater artifacts and `latest.json` for the in-app updater
- This README and [LICENSE](./LICENSE) on the default branch (and attached to each release)

No source code, issues, or pull requests are maintained here.

## Support

For bugs and feature requests, use the project’s private source repository (if you have access) or contact the maintainer.

## License

Binary builds are distributed under the [Repertoire Binary Distribution License](./LICENSE).
