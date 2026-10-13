# Sicode releases

Downloads for **Sicode**, a native macOS worktree terminal for coding agents (Claude Code, Codex).
The source is private; this repository only hosts builds and the update feed.

## Install

```bash
brew install --cask jonasdpdk/tap/sicode
```

or download `Sicode-<version>.dmg` from [Releases](https://github.com/JonasDPDK/sicode-releases/releases) and drag
Sicode to Applications.

Requires macOS 26 on Apple silicon. Sicode isn't notarized: if macOS blocks the first launch, open
**System Settings → Privacy & Security** and click **Open Anyway**. After that Sicode updates itself
(Sparkle, EdDSA-signed `appcast.xml` attached to each release).
