# 0rbe

**0RBE** is an original orbital chain shooter by M.A. Vélez-Guerrero ([@mandresve](mailto:mandresve@hotmail.com)), developed for the Trimui Brick and Trimui Brick Pro and packaged for PortMaster by the author. Special thanks to the PortMaster team and testers for their tooling and support.

Unlike conventional ports, 0RBE is a small native program that generates its entire visual and audio experience at runtime. It draws everything — orbs, skies, black holes, backgrounds and its own typeface — and synthesizes all sound effects and music in real time using the system SDL2 library.

No external game assets, images, audio samples, fonts or additional libraries are bundled.

The first launch asks you to select a language. Available languages are English, Español, Italiano, Français, Deutsch, Português and Nederlands. The language can be changed later in Settings.

The game renders internally at **1024 × 768** and scales to the device display while preserving its original 4:3 aspect ratio.


## Screenshots

<p align="center">
  <img src="cover.png" alt="0RBE - Game Cover" width="48%">
  <img src="shot1.png" alt="0RBE - Gameplay Screenshot" width="48%">
</p>


## Downloads & Installation

0RBE is available in two different packages, depending on your preferred installation method and frontend.

### 1. PortMaster — `0rbe.zip`

**Standard PortMaster autoinstall package.**

This is the recommended package for users running PortMaster on supported handheld devices.

Installation:

1. Download `0rbe.zip`.
2. Transfer the ZIP file to your device's PortMaster installation directory, typically `ports/`.
3. Open PortMaster and select the local installation option.
4. Install 0RBE and wait for the process to finish.
5. Launch the game from your device's Ports menu.

The package includes the necessary PortMaster installation structure and launch scripts.

### 2. Standalone PAK — `0rbe.pak.zip`

**Alternative package for MiniUI, NextUI and NX Redux.**

This package allows 0RBE to be installed as a standalone tool in compatible PAK-based frontend environments.

Supported frontends:

- MiniUI
- NextUI
- NX Redux

Installation:

1. Download `0rbe.pak.zip`.
2. Extract the archive.
3. Locate the included PAK package.
4. Copy it to the appropriate tools or applications directory used by your frontend.
5. Refresh or restart the frontend if necessary.
6. Launch 0RBE from the tools or applications menu.

Refer to your frontend's documentation for the correct installation directory and PAK installation conventions.

### Which package should I use?

| Frontend / Environment | Package |
|---|---|
| PortMaster | `0rbe.zip` |
| MiniUI | `0rbe.pak.zip` |
| NextUI | `0rbe.pak.zip` |
| NX Redux | `0rbe.pak.zip` |

Both packages provide the same game and gameplay experience. The only difference is the installation method and frontend integration.

## Game Features

- **Original orbital chain-shooter gameplay:** An arcade experience built around aiming, shooting and creating orb chains.
- **Procedural graphics:** Orbs, backgrounds, skies, black holes and typography are drawn entirely by the game.
- **Real-time synthesized audio:** All sound effects and music are generated dynamically.
- **Seven languages:** English, Español, Italiano, Français, Deutsch, Português and Nederlands.
- **Scalable rendering:** Internal 1024 × 768 resolution with aspect-ratio-preserving scaling.
- **Persistent progress:** Game progress and settings are saved locally.
- **Minimal dependencies:** Uses the system SDL2 library without bundling external assets or additional runtime libraries.

## Controls

| Button | Action |
|---|---|
| D-Pad | Move the crosshair; navigate menus |
| Left / Right Stick | Move the crosshair (where present) |
| L1 / R1 (hold) | Move the crosshair faster |
| A / R2 | Shoot; confirm |
| B / L2 | Swap the next orb; back |
| Y | Fire the Nova orb (when ready) |
| X (hold) | Precise aim |
| Select | Toggle aim guide on / off |
| L3 / R3 | Center the crosshair (where present) |
| Start / Menu | Pause |
| Start + Select (hold 1 second) | Exit |

Everything can be played using the D-Pad alone.

## Compatibility

0RBE was developed and tested on:

- Trimui Brick
- Trimui Brick Pro

The standalone PAK distribution is intended for compatible MiniUI, NextUI and NX Redux environments.

Compatibility with other devices and firmware versions may depend on their architecture, SDL2 implementation and frontend environment.

## Saves & Configuration

Game progress and settings are stored locally.

- **Save file:** `ports/0rbe/conf/save.txt`
- **Log file:** `ports/0rbe/log.txt`

The save file is created and maintained automatically by the game.

If you experience unexpected behavior, the log file may provide useful information for troubleshooting.

## Technical Details

| Property | Description |
|---|---|
| Architecture | ARM64 (AArch64) |
| Internal resolution | 1024 × 768 |
| Aspect ratio | 4:3 |
| Graphics | Procedurally generated |
| Audio | Real-time synthesized |
| Graphics and audio library | SDL2 |
| External assets | None |
| Additional game data | None |
| Source code | Closed source |

## Compile

0RBE is closed source.

The included `orbe.aarch64` binary is built by the author using the `ghcr.io/loveretro/tg5040-toolchain` Docker image (GCC 8.3, glibc 2.17).

Runtime dependencies:

- `libSDL2-2.0.so.0` (SDL 2.0.18 or newer)
- `libm`
- `libc`

No other external runtime libraries or bundled assets are required.

## Testing & Feedback

0RBE is being tested with the help of the PortMaster community.

For testing reports, bug reports, compatibility feedback, suggestions or general discussion, visit the official **[0RBE Testing Thread on Discord](https://discord.com/channels/1122861252088172575/1571976260857630941)**.

Feedback is always welcome and helps improve the game and its compatibility across devices and frontend environments.

## License & Distribution

0RBE is freeware and is distributed through PortMaster with the author's permission.

The game is provided free of charge for personal enjoyment and distribution through the supported packages.

See `0rbe/licenses/LICENSE.0rbe.txt` for the license and distribution terms.

---

**Created by M.A. Vélez-Guerrero**

[@mandresve](mailto:mandresve@hotmail.com)
