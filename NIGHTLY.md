# Unofficial macOS ARM nightlies

This public fork builds **unsigned** Apple Silicon packages when [`wavetermdev/waveterm`](https://github.com/wavetermdev/waveterm) `main` moves.

## Download

Stable links (same filenames every build; contents refresh when upstream moves):

- [Wave-macos-arm64-nightly.dmg](https://github.com/aloasut/waveterm/releases/download/nightly/Wave-macos-arm64-nightly.dmg)
- [Wave-macos-arm64-nightly.zip](https://github.com/aloasut/waveterm/releases/download/nightly/Wave-macos-arm64-nightly.zip)
- [Release page](https://github.com/aloasut/waveterm/releases/tag/nightly)

## Notes

- After each successful build, the status block at the top of `README.md` is rewritten automatically (commit message includes `[skip ci]`).

- Not affiliated with Command Line Inc / official Wave releases.
- Builds skip code signing and notarization. On first launch macOS may block the app; use right-click → Open, or clear quarantine with `xattr -cr /path/to/Wave.app`.
- Workflow: `.github/workflows/macos-arm-nightly.yml` (every 6 hours; no-op if upstream SHA unchanged). Manual **Run workflow** with `force` rebuilds anyway.

## Trigger manually

Actions → **macOS ARM nightly** → Run workflow.
