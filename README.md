# CraftRoster — WoW Forever guild crafting addon

CraftRoster helps guildmates find crafters, inspect recipes and materials, compare estimated costs, and coordinate requests.

## Choose your download

### 1. CraftRoster addon — game files

**[Download the latest published addon release](https://github.com/hurlburtc-png/CraftRoster-Releases/releases)** and choose **`CraftRoster.zip`**.

Extract into your WoW Forever installation so the file is at `Interface/AddOns/CraftRoster/CraftRoster.toc`. This is the **addon**, not a Windows installer. Do not download GitHub's automatically generated “Source code (zip)”.

### 2. CraftRoster Windows Updater — optional utility

A **separate Windows utility** is under development to find your WoW Forever folder, check for updates, and install or roll back addon versions. Its intended release filename is **`CraftRoster-Windows-Updater.zip`** (or a separately named signed installer in the future).

**Not published or cleared for guild-wide use yet.** Do not mistake `CraftRoster.zip` for the updater or assume the updater is included inside the addon ZIP. The updater will be published as its own clearly labeled download only after Windows testing and security review. The addon works without it.

## Release freshness

Check the release tag and asset list for the current public addon build. Check the Releases page for what is **actually published**; older release assets are not silently overwritten.

## About CraftRoster

- Search recipes, materials, and sources. In beta.114, **Ask Guild** finds crafters through regular chat and saves responders for later. Auto-replies default to on, and `/craskguild` toggles them.
- Materials, estimated crafting costs, shopping lists and work orders.
- Review craft requests before sending. In beta.114, **Cancel request** whispers “Request cancelled.” to the crafter.
- Trade and mail preparation; **the player must manually accept the final trade**.

Target: **WoW Forever 1.60.1 · Interface 16001**. Automated tests use simulated client APIs and do not replace live in-game testing.

See [DOWNLOADS.md](DOWNLOADS.md) for separate installation instructions, [PUBLISHING.md](PUBLISHING.md) for release policy and [LICENSE](LICENSE).
