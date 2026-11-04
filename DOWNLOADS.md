# CraftRoster — download and installation guide

## Download A: CraftRoster addon (`CraftRoster.zip`)

[Open public releases](https://github.com/hurlburtc-png/CraftRoster-Releases/releases) and download the release asset named **`CraftRoster.zip`**. This is the game addon, **not** an installer.

1. Find your WoW Forever installation's `Interface/AddOns` folder.
2. Extract the ZIP so it contains **one** top-level `CraftRoster` folder.
3. Verify `Interface/AddOns/CraftRoster/CraftRoster.toc`; never nest `CraftRoster/CraftRoster`.
4. Restart the game and enable the addon.

Do not download GitHub's automatically generated **Source code (zip)**.

## Download B: Windows Updater (optional; not yet released)

The updater is a **separate Windows program**, not part of `CraftRoster.zip`. Once reviewed and published, it will have its **own explicitly named asset**, such as `CraftRoster-Windows-Updater.zip`, with separate instructions.

Planned controls: auto-detect WoW Forever folders (with Browse fallback), **Check for updates now**, optional startup checks, version history, manual rollback and a pause-auto-update option. Its use is optional. **No updater asset is currently verified as published here.**

Do not run an unknown executable or PowerShell script claiming to be CraftRoster. Only use a clearly identified release asset from this repository; review Windows warnings and signatures.

## Version and integrity

The last verified public addon release is **v0.8.0-beta.97**; newer source releases may not yet be mirrored. Verify the version and `SHA256SUMS.txt` on each published release. Do not assume a release exists merely because the README mentions a future version.

The game addon and Windows utility must each have their **own named asset, version, checksum, release notes and testing status**. Do not bundle the updater into the addon ZIP or the addon into the updater installer.

## Safety and support

The updater should never modify WoW's `WTF/SavedVariables`, run as a service or silently downgrade. CraftRoster never automatically accepts the final trade. Automated tests do not replace native Windows or WoW client acceptance.

Development happens in a separate private repository. See [PUBLISHING.md](PUBLISHING.md) and [LICENSE](LICENSE).
