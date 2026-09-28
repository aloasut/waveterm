# Unofficial macOS ARM nightlies

This public fork builds **unsigned** Apple Silicon packages when [`wavetermdev/waveterm`](https://github.com/wavetermdev/waveterm) `main` moves.

## Download

See the rolling **[nightly](../../releases/tag/nightly)** prerelease (assets replaced on each successful build).

## Notes

- Not affiliated with Command Line Inc / official Wave releases.
- Builds skip code signing and notarization. On first launch macOS may block the app; use right-click → Open, or clear quarantine with `xattr -cr /path/to/Wave.app`.
- Workflow: `.github/workflows/macos-arm-nightly.yml` (every 6 hours; no-op if upstream SHA unchanged). Manual **Run workflow** with `force` rebuilds anyway.

## Trigger manually

Actions → **macOS ARM nightly** → Run workflow.
