# kram-bin

Arch Linux AUR packaging for the prebuilt `kram` CLI release.

Upstream `kram` is a command-line tool for working with KTX, KTX2, DDS, and related texture formats. This repo only contains the AUR packaging needed to install the upstream Linux binary cleanly on Arch.

## How It Works

The `PKGBUILD` downloads the release archive `kram-linux.zip`, extracts the `kram` executable, and installs it to `/usr/bin/kram`. If the archive contains a license file, it is installed too.

## Install locally

```bash
makepkg -si
```

## Notes

- Packaging-only repository: no upstream source code is vendored here.
- Current package target is `x86_64`.
- The package currently tracks upstream version `1.7.30`.
- Main files are `PKGBUILD` and `.SRCINFO`.
