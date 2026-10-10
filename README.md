# minecraft!(lazer)

osu!lazer's interface for Minecraft: the intro, main menu, settings, overlays, chat and friends, rebuilt from osu!lazer's own source.

This repository holds the releases. Download the latest version from the [Releases page](https://github.com/Xaikaw/minecraft-lazer-releases/releases/latest).

## Install

1. Install [Fabric Loader](https://fabricmc.net/use/installer/) 0.17 or newer for **Minecraft 1.21.11**.
2. Put [Fabric API](https://modrinth.com/mod/fabric-api) in your `mods` folder.
3. Download `minecraft-lazer-<version>-mc1.21.11.jar` from the latest release and put it in your `mods` folder.
4. Start Minecraft with the Fabric profile.

osu! doesn't need to be installed. If it is, your beatmaps play as menu music.

## Updates

minecraft!(lazer) keeps itself up to date, like osu!lazer:

1. When the game starts, and every 30 minutes after, it looks for a new release here.
2. A new version downloads in the background. It's checked against the SHA-256 published with the release, and the game also checks it's the right mod, version and Minecraft version.
3. **Update ready to install. Click to restart!** Click to restart into the new version now, or it installs the next time you close the game.

Only the mod's jar is replaced. Your settings and worlds stay as they are.

**Release streams** (Settings > General > Updates):

| Stream | What you get |
|---|---|
| **Stable** | Regular releases |
| **Beta** | Pre-releases as well, so you get new things first (they may be less polished) |

Going back to Stable moves you to the latest stable release.

**If an update causes trouble:** go to Settings > General > Updates and use **Restore previous version**. The jar you had before the last update is kept in `.minecraft/osumenu/updates/backup/`.

## Verifying a download yourself

Every release has a `.sha256` file next to its jar, and GitHub shows each file's SHA-256 too. On Windows:

```bash
certutil -hashfile minecraft-lazer-0.2.0-mc1.21.11.jar SHA256
```

## Problems and ideas

Open an [issue](https://github.com/Xaikaw/minecraft-lazer-releases/issues) and include:
- your minecraft!(lazer) version (Settings > General > Updates shows it);
- your `logs/latest.log`;
- what happened.

---

osu! assets (fonts, sounds, textures) are by ppy Pty Ltd under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). minecraft!(lazer) isn't affiliated with or endorsed by ppy, Mojang or Microsoft.
