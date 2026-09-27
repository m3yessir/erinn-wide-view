# m3yessir's Erinn Wide View — Mabinogi FOV Mod

**By m3yessir · v0.2.0-beta · Mabinogi North America**

A file-based mod that sets the camera FOV to **110 in supported towns, fields, and dungeon instances**. It widens the viewing angle while keeping the game's stock zoom limits. No DLL injection is used.

**[Download from Releases](https://github.com/m3yessir/erinn-wide-view/releases)** — choose the attached `m3yessir-Erinn-Wide-View-v0.2.0-beta.zip` under Assets.

## Where it works

- **Towns and fields:** supported regions include Tir Chonaill, Dunbarton, Emain Macha, Tara, and the main Iria fields.
- **Bri Leith:** included since v0.1.0.
- **Glenn Bearna:** included since v0.1.0.
- **Crom Bás:** added in v0.2.0.
- **Homestead and Moonlight Island:** includes the region files listed in [modified-files.txt](modified-files.txt).

Coverage depends on the map, not simply whether it is indoors or outdoors. The package contains **176 region files**, but that does not mean every location, difficulty, or boss camera is supported.

## What's new in v0.2.0?

**Crom Bás now has 110 FOV in the same package.** All 175 previously included region files, including Bri Leith and Glenn Bearna, are unchanged. You no longer need the separate Crom Bás FOV add-on.

## Known limits

- **Generated dungeon rooms**, such as the rooms beyond Ciar's lobby, are not covered.
- **Shops and other building interiors** keep their original camera settings. Earlier experimental changes caused black rendering in Tir shops and were removed.
- **Cutscenes and special cameras** may override the FOV.
- Not every included map, difficulty, or boss room has been tested. This is a beta; report the exact location if something looks wrong.

The **Sidhe visibility/fog mod is separate**. Its haze changes are not included here, and it can stay installed alongside Wide View.

## Install

1. Close Mabinogi completely.
2. Remove the old `m3yessirErinnWideView110_00001.it` and the separate `m3yessirCromBasFov110_00001.it`, if installed. Also remove any older Wide View or `CustomErinnFov110_*.it` / `CustomDunbartonFov*.it` test packages. Keep backups outside the active package folder.
3. Check for conflicting mods listed below.
4. Copy **`m3yessirErinnWideView110_00002.it`** into the game's active package directory: the folder containing the official `data_00000.it`, `data_00001.it`, etc. archives.
5. Restart the game.

Install layouts vary. The active directory may be `Mabinogi\package` or `Mabinogi\appdata\package`. Use the existing directory containing the game's `.it` archives.

**Do not rename the `.it` file.** Its archive metadata depends on its final filename. Keep only one version installed.

Findias does not automatically install or update this standalone release from its normal Uiscias catalog.

## Conflicts

**If you use Findias, disable any of these mods before installing Erinn Wide View:**

- **Bri Leith Zoom And FoV** — both 60 and 90 versions.
- **Crom Bas Zoom And FoV And Declutter** — both 60 and 90 versions.
- **Farm WASD Bug Fix** — both versions, including **No FoV**.
- **Glenn Bearna Zoom** — all four versions, with or without Declutter.
- **Homestead Zoom And FoV**.
- **Moonlight Island Zoom And FoV**.

They edit the same map files as Erinn Wide View, so one mod can override the changes made by another. Disabling them means losing their extra zoom, decluttering, or bug fixes; Erinn Wide View does not include those features.

Erinn Wide View works on its own. You do not need to install any of the mods above.

List checked against Uiscias v1.65.0 on September 26, 2026. For exact file matches and technical details, see [CONFLICTS.md](CONFLICTS.md).

## Remove

Close the game, remove this `.it` from the active package directory, and restart. Re-enable any mods you disabled specifically for this installation. Original game archives are not overwritten.

## Build and verification

Built from a North American Steam installation, build **25329795**, on **2026-09-26**. A later game update may change region data and require a new mod build.

- 176 region entries; all entry paths and archive metadata validated.
- Every extracted file matched the intended size and SHA-256 hash.
- The 175 previously included region files and one Crom Bás file exactly match their previously verified packages. All 176 region structures parsed successfully; the underlying XML edits are limited to FOV and, where needed in the original build, the camera-override enable flag.
- Stock zoom limits, existing near/far-distance numbers, lighting and other XML settings were preserved.

Where the existing camera override was disabled, it is enabled to apply the FOV. That can also activate the region's stored distance settings, so rendering behavior still needs in-game testing.

Package size: **422,841 bytes**.

SHA-256:

`64981428730894fb4b2ad367b4c4f6e608ca069aab33bcf1468dd4eb9043e7f8`

See `release-manifest.json`, `SHA256SUMS.txt` and `CREDITS.md` for details.

## Report a problem

Include the location, whether it is outdoors/indoors/a generated dungeon, mod version, game version, and any other installed map or camera mods. A before/after comparison at the same resolution, position and zoom helps identify camera changes.
