# m3yessir's Erinn Wide View

**By m3yessir · v0.1.0-beta · Mabinogi North America**

A standalone, file-based mod that requests a wider 110-degree camera field of view in supported outdoor regions. No DLL injection is used.

The package edits 175 outdoor region files and templates. It preserves their stock zoom limits and stored distance values. It does not bundle other gameplay, interface, or zoom mods.

## Scope

- Covers outdoor regions including Tir Chonaill, Dunbarton, Emain Macha, Tara and the main Iria fields. See `modified-files.txt` for the exact paths.
- Leaves building interiors unchanged. Experimental interior overrides were removed after they caused black rendering in Tir Chonaill shops.
- Does not solve FOV in generated dungeon rooms, such as the rooms beyond Ciar's lobby.
- Does not modify cutscene scripts, mission-variation camera XML, or login/character-selection screens. Special cameras and mission variants can still override the view.
- Skips outdoor regions without the existing camera attributes needed for this version.

The earlier personal build was tested in many towns, and the interior rollback was confirmed working by its tester. This standalone beta is derived from that build, but it is not a claim that every included region has been tested or that the engine's numerical FOV has been measured.

## Install

1. Close Mabinogi completely.
2. Remove older versions of this mod and any `CustomErinnFov110_*.it` or `CustomDunbartonFov*.it` test packages from the active package directory.
3. Check for conflicting mods listed below.
4. Copy **`m3yessirErinnWideView110_00001.it`** into the game's active package directory: the folder containing the official `data_00000.it`, `data_00001.it`, etc. archives.
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

- 175 region entries; all entry paths and archive metadata validated.
- Every extracted file matched the intended size and SHA-256 hash.
- All edited region XML parsed successfully; semantic changes were restricted to FOV and the camera-override enable flag.
- Stock zoom limits, existing near/far-distance numbers, lighting and other XML settings were preserved.

Where the existing camera override was disabled, it is enabled to apply the FOV. That can also activate the region's stored distance settings, so rendering behavior still needs in-game testing.

Package size: **420,793 bytes**.

SHA-256:

`48ad03d7643559d6f6520c34e3c6a14bb964e2441a873d463ad01b1be726be46`

See `release-manifest.json`, `SHA256SUMS.txt` and `CREDITS.md` for details.

## Report a problem

Include the location, whether it is outdoors/indoors/a generated dungeon, mod version, game version, and any other installed map or camera mods. A before/after comparison at the same resolution, position and zoom helps identify camera changes.
