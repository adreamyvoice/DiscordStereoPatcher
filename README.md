# Discord Stereo Patcher (macOS)

Patches Discord's voice module on macOS for true stereo, 48 kHz, 384 kbps audio with adjustable gain.

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
- Xcode Command Line Tools (run `xcode-select --install` if you don't have them)

## Credits

Made by **Voice**.

> ⚠️ Modifies Discord files. Use at your own risk. Re-run after Discord updates. Not affiliated with Discord Inc.
