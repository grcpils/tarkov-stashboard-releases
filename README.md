<p align="center">
  <img src="icon.png" width="96" alt="Tarkov Stashboard icon" />
</p>

<h1 align="center">Tarkov Stashboard</h1>

<p align="center">
  A free desktop companion for <b>Escape from Tarkov</b>.<br />
  Track your quests, read the wiki guide next to each one, plan your Hideout, and know which items to keep.
</p>

<p align="center">
  <a href="https://github.com/grcpils/tarkov-stashboard-releases/releases/latest"><b>Download the latest version</b></a>
</p>

---

> Tarkov Stashboard is a fan-made tool. It is not affiliated with, endorsed by, or connected to Battlestate Games. It only reads the game's log files: it never reads game memory, never draws over the game, and never touches the game client.

This repository hosts the downloads and the automatic updates of the app. It contains no source code.

## Download

Go to the [latest release](https://github.com/grcpils/tarkov-stashboard-releases/releases/latest) and pick one file:

| File | Pick it when |
|---|---|
| `Tarkov-Stashboard-Setup-<version>.exe` | **Recommended.** A normal install: one click, no administrator rights, with a shortcut, an uninstaller and automatic updates. |
| `Tarkov-Stashboard-Portable-<version>.exe` | You do not want to install anything. It is a single file that starts more slowly and does not update itself. |

You can ignore `latest.yml` and the `.blockmap` file: the app uses them to update itself.

Requirements: Windows 10 or 11, 64-bit.

### "Windows protected your PC"

The app is not code-signed, so Windows SmartScreen shows this warning the first time you run it. Click **More info**, then **Run anyway**.

## What it does

| Screen | What you get |
|---|---|
| **Overview** | Your PMC level, pinned and active quests, the maps where you have the most to do, the top items to keep, and the quests that unlock soon. |
| **Quests** | Every quest with its status: available, active, completed, failed, locked or uncertain. Search, filters by trader, map and status, and a grouping by map to plan a raid. |
| **Quest page** | Objectives you can tick, required items and keys, rewards, and the "Guide" section of the wiki with its images. |
| **Maps** | Interactive maps with floors, quest markers and extracts. |
| **Hideout** | A top-down plan of the Hideout. Each module shows its level, what it needs, and whether you can build it. |
| **Keep list** | Every item your quests and Hideout upgrades need, with quantities, found-in-raid requirements and what you already own. |

Also:

- **Automatic quest tracking.** The app reads the game's logs and ticks your quests for you.
- **PvE and PvP** are tracked separately.
- **English and French** interface, including quest, item and map names.
- **Works offline** once the game data is downloaded.

## Getting started

1. Install and open the app.
2. In **Settings**, pick your game mode (PvE or PvP) and your faction.
3. Still in **Settings**, link the game's `Logs` folder. The app usually finds it on its own and offers it.
4. If you wiped recently, set the wipe date so that older quests are ignored.

From then on, quests you accept, complete or fail in game are updated in the app. The game writes these changes outside of raids, so a quest completed in raid shows up once you are back in the menus.

Some quests are marked **uncertain**: their unlock conditions are not in the public data, so the app cannot tell whether you have them. Click **I have it** when you do.

## Automatic updates

The installed version keeps itself up to date:

- it looks for a new version at startup and every four hours;
- it downloads it in the background and checks the file's integrity;
- a **Version x.y.z ready: restart** button appears in the bottom bar. Click it, or just close the app: the update installs on exit.

**Settings > Application** shows your version and a **Check for updates** button. The portable version does not update itself: download the new file here.

## Privacy

- No account, no telemetry, no ads.
- Your progress stays on your computer, in `%APPDATA%\TarkovStashboard`.
- The game's `Logs` folder is opened read-only, and nothing from it is sent anywhere.
- The app only connects to tarkov.dev (game data, icons, maps), the Escape from Tarkov wiki (quest guides) and GitHub (updates).

To move your progress to another computer, use **Settings > Backup** to export it as a file, then import it there.

## Uninstall

Open **Windows Settings > Apps > Installed apps**, find Tarkov Stashboard and uninstall it. Your progress is kept. To remove it too, delete the `%APPDATA%\TarkovStashboard` folder.

## Problems and suggestions

Found a bug or have an idea? [Open an issue](https://github.com/grcpils/tarkov-stashboard-releases/issues). Please include the app version (shown in the bottom-left corner) and what you were doing.

Wrong quest data (a requirement, a level, a reward) usually comes from the upstream data. Try **Settings > Update game data** first.

## Credits

Tarkov Stashboard only exists thanks to community projects. None of them is affiliated with this app.

| Source | What comes from it |
|---|---|
| [tarkov.dev](https://tarkov.dev) ([the-hideout](https://github.com/the-hideout)) | Quests, Hideout, items, traders, icons, interactive maps (MIT-licensed code and map settings) |
| [Escape from Tarkov Wiki](https://escapefromtarkov.fandom.com) (Fandom) | Quest guides and their images, under [CC BY-NC-SA](https://www.fandom.com/licensing), with a link back to each page |
| [tarkov-data-overlay](https://github.com/tarkovtracker-org/tarkov-data-overlay) (tarkovtracker-org) | Community corrections to quest requirements (MIT) |
| Community map authors, via tarkov.dev | 2D map images, credited under each map in the app |
| [Rajdhani](https://fonts.google.com/specimen/Rajdhani) (Indian Type Foundry) | Interface font (SIL Open Font License 1.1) |

## Legal

Escape from Tarkov and all related names, images and game content are trademarks or property of **Battlestate Games Limited**. This is an unofficial fan tool, free and with no commercial purpose.

The app is provided as is, without warranty of any kind.
