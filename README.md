# Discord Stereo Patcher (macOS)

Patches Discord's voice module on macOS for true stereo, 48 kHz, 384 kbps audio with adjustable gain.

## Before you start — read this

- **Disable SIP (System Integrity Protection)** on your Mac before patching. If SIP is on, Discord won't let you connect to voice chat after the patch is applied.
  How: reboot into Recovery (Apple menu → Restart, hold the power button on Apple Silicon, or ⌘R on Intel) → open **Terminal** from the Utilities menu → run `csrutil disable` → reboot.
- **Install both Xcode and the Xcode Command Line Tools** before running the patcher.
  - Xcode: install from the App Store.
  - Command Line Tools: open Terminal and run `xcode-select --install`.

Without these two steps the patch will either fail to build or fail to connect to voice.

## Install

1. Click **Code → Download ZIP** (or `git clone` this repo).
2. Open `DiscordStereoPatcher.app`.
3. The first time, macOS may say it's from an unidentified developer — right-click the app and pick **Open**, then **Open** in the dialog.

## What it does

- Closes Discord
- Backs up the existing voice module
- Applies binary patches to enable stereo + high bitrate
- Restarts Discord

You can hit **Restore** in the GUI to roll back any time.

## Requirements

- macOS 14 (Sonoma) or newer
- **SIP disabled** (see the warning at the top)
- **Xcode** (App Store) and **Xcode Command Line Tools** (`xcode-select --install`)

## Credits

Made by **Voice**.

> Modifies Discord files. Use at your own risk. Re-run after Discord updates. Not affiliated with Discord Inc.
