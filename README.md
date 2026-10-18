# Sicode releases

Downloads for **Sicode**, a native worktree terminal for coding agents (Claude Code, Codex and others) on macOS and
Windows. The source is private; this repository only hosts builds and the update feeds.

## macOS

```bash
brew install --cask jonasdpdk/tap/sicode
```

or download `Sicode-<version>.dmg` from [Releases](https://github.com/JonasDPDK/sicode-releases/releases) and drag
Sicode to Applications.

Requires macOS 26 on Apple silicon. Sicode isn't notarized: if macOS blocks the first launch, open
**System Settings → Privacy & Security** and click **Open Anyway**. After that Sicode updates itself
(Sparkle, EdDSA-signed `appcast.xml` attached to each release).

## Windows

Download `SicodeApp-win-Setup.exe` from the newest release that has it in
[Releases](https://github.com/JonasDPDK/sicode-releases/releases) and run it. `SicodeApp-win-Portable.zip` runs
without installing.

Requires Windows 11 x64 (or Windows 10 22H2); the installer brings the .NET 10 desktop runtime when it's missing.
The installer isn't signed yet: if SmartScreen stops it, click **More info → Run anyway**. After that Sicode updates
itself (Velopack, from `releases.win.json` and the `SicodeApp-*.nupkg` packages attached to each release).

Some releases carry only one platform's files; each app finds its own newest update.
