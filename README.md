# Breeze Aion DPS Meter

A Windows companion for AION 2 with a live encounter overlay, saved encounter logs, interactive maps, and boss timers.

This repository hosts installers, release notes, and distribution notices. Application source code is not included.

## Download the preview

[Download 0.2.1 Preview](https://github.com/tafelfish/Breeze-Aion-DPS-Meter/releases/tag/v0.2.1)

Download `Aion2Meter_0.2.1_x64-setup.exe` from the release assets and run it. The installed application and shortcuts are currently named **Aion 2 Meter**. Existing installations retain their settings and encounter history when upgraded.

Requirements:

- Windows 10 or 11, 64-bit.
- [Npcap](https://npcap.com/#download) installed separately for live capture.
- Microsoft Edge WebView2 Runtime. Setup downloads it if it is missing.
- Internet access for character profiles, remote images, and GitHub update checks.

The preview installer is unsigned. Windows may display an unknown publisher or SmartScreen warning.

## Included

- Automatic game connection detection and encounter recording.
- A customizable overlay with click-through anchoring and a configurable hotkey.
- Damage, healing, damage taken, skill breakdowns, timelines, and captured buff uptime.
- Encounter history grouped by dungeon run, with newest encounters first.
- Character profiles and progression suggestions.
- Interactive maps with saved layer choices and collection markers.
- Boss timers, favorites, and configurable notifications.
- Optional Windows startup and update notifications.

Capture coverage depends on available game messages. Missing cast, buff, identity, or profile data can leave statistics incomplete. Game updates may change capture behavior. This is a preview, and measurements are not guaranteed to match the game exactly.

## Updates

The app checks this repository's latest **production release** and the local update folder on startup and every 15 minutes. It offers installation through Settings and notifies you in the overlay. It does not install updates automatically or intentionally interrupt an active encounter.

GitHub prereleases are excluded from automatic checks. Download preview releases manually from this repository. After installing 0.2.1, the next production update must have a higher version to be offered. GitHub update checks do not require a GitHub account.

Installer downloads are checked against the release manifest's size and SHA-256. `latest.json` is update metadata; you only need to run the setup executable.

## Data and notices

Encounter logs and settings are stored locally. Live capture reads game connection traffic; it does not capture the screen or read game process memory. Character lookup and image requests use external game services. Update checks contact GitHub. Raw packet recordings are not uploaded by the meter.

This project is independent and is not affiliated with or endorsed by NCSOFT. Game names and artwork belong to their respective owners. Included map data is licensed for noncommercial use. See [distribution notices](notices/distribution-notices.txt) and [map and catalog notices](notices/companion-notices.txt).
