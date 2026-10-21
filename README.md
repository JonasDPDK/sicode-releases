# Monnercode releases

Downloads for **Monnercode**, a native worktree terminal for coding agents (Claude Code, Codex and others) on macOS
and Windows. The source is private; this repository only hosts builds and the update feeds.

Monnercode was called **Sicode** up to v0.9.7, and those releases carry the old name. Installed Sicode copies
update to Monnercode by themselves and move their settings over on the first launch.

## macOS

```bash
brew install --cask kodeance/tap/monnercode
```

or download `Monnercode-<version>.dmg` from [Releases](https://github.com/Kodeance/monnercode-releases/releases)
and drag Monnercode to Applications.

Requires macOS 26 on Apple silicon. Monnercode isn't notarized: if macOS blocks the first launch, open
**System Settings → Privacy & Security** and click **Open Anyway**. After that Monnercode updates itself
(Sparkle, EdDSA-signed `appcast.xml` attached to each release).

## Windows

Download `MonnercodeApp-win-Setup.exe` from the newest release that has it in
[Releases](https://github.com/Kodeance/monnercode-releases/releases) and run it. `MonnercodeApp-win-Portable.zip`
runs without installing.

Requires Windows 11 x64 (or Windows 10 22H2); the installer brings the .NET 10 desktop runtime when it's missing.
The installer isn't signed yet: if SmartScreen stops it, click **More info → Run anyway**. After that Monnercode
updates itself (Velopack, from `releases.win.json` and the `MonnercodeApp-*.nupkg` packages attached to each
release).

Some releases carry only one platform's files; each app finds its own newest update.
