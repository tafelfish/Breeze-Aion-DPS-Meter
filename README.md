# Breeze Aion DPS Meter

A Windows companion for AION 2 with a live encounter overlay, saved encounter logs, interactive maps, and boss timers.

This repository hosts installers, release notes, and distribution notices. Application source code is not included.

## Download

[Download 1.3.3](https://github.com/tafelfish/Breeze-Aion-DPS-Meter/releases/tag/v1.3.3)

Download `Aion2Meter_1.3.3_x64-setup.exe` from the release assets and run it. The installed application and shortcuts are named **Aion 2 Meter**. Existing users can select **Check for updates** in Companion Settings. Upgrades retain settings and encounter history.

Requirements:

- Windows 10 or 11, 64-bit.
- [Npcap](https://npcap.com/#download) installed separately for live capture.
- Microsoft Edge WebView2 Runtime. Setup downloads it if it is missing.
- Internet access for character profiles, remote images, and GitHub update checks.

The installer is unsigned. Windows may display an unknown publisher or SmartScreen warning.

## Included

- Automatic game connection detection and encounter recording.
- A customizable overlay with click-through anchoring, recorded keyboard shortcuts, game-focused visibility, and optional automatic fades around boss encounters.
- Damage, healing, damage taken, skill breakdowns, timelines, CPM/HPM, and captured buff uptime.
- Optional character power and item level, player privacy controls, and opt-in personal performance comparisons.
- Encounter history grouped by dungeon run, with newest encounters first.
- Character profiles, equipment details, progression suggestions, and compact character/skills PNG exports.
- Saved character sheets and speciality descriptions, with unconfirmed selections marked as unknown.
- Interactive maps with saved layer, gatherable, and pet genus filters and collection markers.
- Boss timers, favorites, and configurable notifications, including a fixed screen position.
- Automatic pet collection tracking, faction completion totals, and a compact nearby pet progress window with completion highlights and chimes.
- A dedicated Edit UI menu with sample data in the actual overlay windows and Save or Cancel controls.
- Character-specific skill reminders with buff-duration or cooldown timers, optional blinking, and dungeon-entry reminders.
- A Black Cloud Merchant window showing unfinished pet offers, with an optional Unfarmable Pets only filter.
- Fresh nearby pet distances, a pet tracker visibility shortcut, and completed-pet map markers.
- Scheduled reminders for Shugo Festival, Dimensional Invasions and Spacetime Rifts.
- Up to three additional meter windows with independent metrics and appearance.
- Timed training, encounter comparisons, selectable ranges and encounter images copied to the clipboard.
- Layout profiles, collapsible editing controls, portable settings and custom notification sounds.
- An experimental crafting tree with owned-material deductions, planning scenarios and marketplace prices.
- PvE gear stat priorities and personal desired-stat targets.
- Experimental restored-healing measurements with explicit unknown events and partial coverage.
- Server ping on the meter or in a transparent window, with color indicators and optional 60-second history.
- Undo/Redo while editing layouts and settings search with direct navigation.
- Optional Windows startup and update notifications.

Restored-healing coverage is still limited; totals may be incomplete. Crafting prices and supported success rates depend on available data.

Capture coverage depends on available game messages. Missing cast, buff, identity, or profile data can leave statistics incomplete. Game updates may change capture behavior. Measurements are not guaranteed to match the game exactly. Speciality selections remain unknown when they cannot be confirmed; description values may vary by game version.

## Updates

The app checks this repository's latest **production release** and the local update folder on startup and every 15 minutes. It offers installation through Settings and notifies you in the overlay. It does not install updates automatically or intentionally interrupt an active encounter.

GitHub prereleases are excluded from automatic checks. Version 1.3.3 is a production release and is available to earlier versions through the updater. Future production releases with a higher version will be offered in the same way. GitHub update checks do not require a GitHub account.

Installer downloads are checked against the release manifest's size and SHA-256. `latest.json` is update metadata; you only need to run the setup executable.

## Data and notices

Encounter logs and settings are stored locally. Live combat capture reads game connection traffic and does not read game process memory. Character lookup and image requests use external game services. Update checks contact GitHub. Raw packet recordings are not uploaded by the meter.

This project is independent and is not affiliated with or endorsed by NCSOFT. Game names and artwork belong to their respective owners. Included map data is licensed for noncommercial use. See [distribution notices](notices/distribution-notices.txt) and [map and catalog notices](notices/companion-notices.txt).
