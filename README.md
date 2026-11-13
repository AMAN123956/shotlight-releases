# Shotlight

Shotlight names every screenshot the moment you take it, and finds any of them by the words inside (⌥Space).
Everything runs on your Mac. No account, no analytics, and it never connects to the internet.

This repository only holds the downloads and the bug tracker. There's no source code here.

## Download

**[Download Shotlight (latest)](https://github.com/AMAN123956/shotlight-releases/releases/latest/download/Shotlight.dmg)** · [All versions and release notes](https://github.com/AMAN123956/shotlight-releases/releases)

Needs a Mac with **Apple silicon** and **macOS 15** or later. On macOS 26 with Apple Intelligence turned on, names
are richer. Otherwise Shotlight names each screenshot from the text it reads in it.

## Opening it the first time

This early build isn't signed by Apple yet, so macOS asks you to confirm it once:

1. Open the `.dmg` and drag **Shotlight** to **Applications**.
2. Open Shotlight. macOS says it can't verify the app. Click **Done** (not Move to Trash).
3. Open **System Settings › Privacy & Security**, scroll down and click **Open Anyway** next to Shotlight. Confirm with
   your password.
4. Shotlight appears in the menu bar and walks you through setup.

If you prefer Terminal: `xattr -dr com.apple.quarantine /Applications/Shotlight.app`

You do this once per version. After an update, macOS may also ask again for access to your Desktop. Both go away
once Shotlight is signed by Apple.

## Updating

Shotlight never checks for updates by itself, because it never goes online. To update, download the latest version
and replace the app in Applications. Your names, search index and settings are kept.

## Bugs and ideas

[Open an issue](https://github.com/AMAN123956/shotlight-releases/issues/new/choose). If you attach a screenshot,
blur anything private first.

## Privacy

Shotlight collects nothing. Your screenshots, the text read from them and the search index stay in
`~/Library/Application Support/Shotlight` on your Mac. Naming uses Apple Vision and, where available, Apple
Intelligence, both on-device.
