# scoop-airglass

[Scoop](https://scoop.sh) bucket for [AirGlass](https://github.com/jdkuk/AirGlass), a free,
open-source (GPL-3.0) AirPlay receiver for Windows 10/11.

AirGlass mirrors an iPhone, iPad or Mac to a floating window on a Windows PC over AirPlay, and
plays AirPlay music in lossless (Apple Lossless) quality. See
[jdkuk.github.io/AirGlass](https://jdkuk.github.io/AirGlass/) for details.

This is a personal bucket, not the main Scoop bucket or `extras`, because AirGlass doesn't yet
meet the `extras` bucket's notability bar (see `ScoopInstaller/Extras` CONTRIBUTING.md for the
current criteria). Once it does, the manifest here can be submitted there instead.

## Install

```powershell
scoop bucket add airglass https://github.com/jdkuk/scoop-airglass
scoop install airglass
```

## Update

```powershell
scoop update airglass
```

## Notes

- The manifest uses Scoop's `innosetup` extraction against the official per-user Inno Setup
  installer published on the [GitHub releases page](https://github.com/jdkuk/AirGlass/releases) —
  nothing is repackaged or rehosted.
- The SHA256 hash in `bucket/airglass.json` matches `SHA256SUMS.txt` published with each release.
- `checkver`/`autoupdate` are wired to the GitHub releases feed so `scoop update` picks up new
  AirGlass versions automatically after a release.
