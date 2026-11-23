# Kerr

Real-time relativistic ray tracing of black holes, for the desktop.

Kerr traces the path of light around a black hole on the GPU, pixel by pixel, using general
relativity. The shadow, the photon ring, the lensed accretion disk and the distorted star field
come out of the physics instead of being painted on.

- Schwarzschild (non-rotating) and Kerr (rotating) black holes.
- Thin accretion disk with gravitational and Doppler shifts and relativistic beaming.
- Scientific mode (quantitative, physical) and Cinematic mode (filmic look, labelled where artistic).
- Geodesic inspector: Ctrl + click any pixel to see the path of its light ray.
- Saved scenes, keyboard shortcuts (F1 for help) and a built-in update check.

This repository only hosts the downloads. **Get the latest version from
[Releases](https://github.com/martinezmarcos/kerr-releases/releases/latest).**

## Install on Linux (x86_64)

Requirements: a GPU with a Vulkan driver (`vulkaninfo` should list it), Wayland or X11.

```sh
tar xzf black-hole-lab-<version>-x86_64-linux.tar.gz
cd black-hole-lab-<version>-x86_64-linux
./install.sh            # for your user; then open "Kerr" from the application launcher
```

System-wide: `sudo ./install.sh --prefix /usr/local`. Uninstall: `./install.sh --uninstall`.

## Run on Windows (10/11, 64-bit)

Requirements: a GPU with DirectX 12 or Vulkan and an up-to-date graphics driver.

Download `Kerr-<version>-windows-x64.exe` and double-click it. It is a single portable file:
nothing to install, and it can live in any folder. The `…-x86_64-windows.zip` holds the same exe
plus a README.

The exe is not code-signed, so Windows SmartScreen warns the first time: choose
**More info › Run anyway**. Settings and scenes are kept in `%APPDATA%\black-hole-lab\` and
screenshots (F12) in `Pictures\Kerr\`. To uninstall, delete the exe and those folders. The in-app
update is Linux-only; on Windows, F1 › About tells you when a new version is out and links to it.

## Updates

Kerr checks this repository for a newer release when it starts (you can turn that off in
F1 › About, or check manually there). When one is available it shows a link to download it;
it never installs anything by itself. To update, download the new archive and run `./install.sh`
again: your settings and saved scenes are kept.
