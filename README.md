# m3yessir’s Erinn Wide View — Standalone 110 FOV

**v0.3.0-beta · Mabinogi North America · No Mooncrest installation required**

A file-based `.it` mod that sets FOV to **110** in supported outdoor maps and fixed interiors. It uses no DLL injection and keeps stock zoom-limit fields. This is the fixed-110 standalone download; Mooncrest provides the optional adjustable slider.

## Download

[Download v0.3.0-beta](https://github.com/m3yessir/erinn-wide-view/releases/tag/v0.3.0-beta) and choose **m3yessir-Erinn-Wide-View-v0.3.0-beta.zip** under Assets. GitHub’s Source code ZIP does not contain the installable mod.

## What’s new

- Adds **254 more fixed indoor region files and 63 room-variation files** to the previous standalone release.
- Includes Tara Castle’s Arcana Association, Great Hall and Guild Hall, supported shops, houses and dungeon lobbies.
- Preserves all **176 existing region files byte-for-byte**, including Crom Bás, Bri Leith and Glenn Bearna.
- Contains **493 entries: 430 region files and 63 room-variation XML files**. The indoor coverage totals 255 regions because Crom Bás was already included.

The new indoor files exactly match the expanded FOV payload used in Mooncrest. Selected castle rooms, lobbies and other interiors were tested in game by the maintainer; not every included map has been individually tested.

## Install or update

1. Close Mabinogi completely.
2. Move your previous Wide View `.it` and any conflicting FOV test packages outside the game’s package folder. Keep only one version installed.
3. Check the conflict list below.
4. Extract the download and copy **m3yessirErinnWideView110_00003.it** into the active game `package` folder containing the official `data_*.it` archives.
5. Restart Mabinogi.

**Do not rename the `.it` file.** Its archive metadata depends on its filename. Do not delete or replace the official `data_*.it` archives. Install layouts vary; use the existing package folder for your active game installation.

This standalone mod is updated manually through this repository. It is separate from Mooncrest and does not include Mooncrest or Rua. If you already use Mooncrest’s Global FOV Override, use its slider instead of adding this package.

## Compatibility

Disable overlapping Findias/Uiscias mods before installing this standalone package:

- **Bri Leith Zoom And FoV** — all listed variants.
- **Crom Bas Zoom And FoV And Declutter** — all listed variants.
- **Dungeon Statue Fix** — all listed variants.
- **Farm WASD Bug Fix** — all listed variants.
- **Glenn Bearna Zoom And FoV** — all listed variants.
- **Homestead Zoom And FoV** — all listed variants.
- **Moonlight Island Zoom And FoV** — all listed variants.
- **Phantasm Zoom And Delag** — all listed variants.

Disabling these can remove their extra zoom, decluttering or bug fixes; this package does not include those features. See [CONFLICTS.md](CONFLICTS.md) for exact variants and shared paths, checked against Uiscias v1.65.0. Other mods replacing the same files can also conflict.

## Known limits

- **Generated dungeon combat rooms**, including Peaca’s generated floors, are not covered. A working lobby does not imply the whole dungeon works.
- Cutscenes and special cameras may override FOV.
- Older interiors without complete camera-distance settings use a 7000/7000 override, following the approach tested in the Great Hall and Guild Hall. Other interiors preserve available stock distances. Enabling these settings can change camera behavior.
- Stock render-distance, lighting, geometry and zoom-limit fields are preserved by the indoor edits. Not every map, difficulty or special camera has been tested.
- The source snapshot is the previously tested September 2026 NA game data. This is not a compatibility claim for later game patches.

## Remove

Close the game, remove `m3yessirErinnWideView110_00003.it` from the package folder, and restart. Re-enable mods you disabled for this installation. Original game archives are not overwritten.

## Verification and credits

All 493 entries were packed and extracted again with matching SHA-256 hashes. All region structures parsed, all intended camera FOV values are 110, and the original 176 region payloads are unchanged. See [release-manifest.json](release-manifest.json), [modified-files.txt](modified-files.txt), [SHA256SUMS.txt](SHA256SUMS.txt), and [CREDITS.md](CREDITS.md).

Built with mabi-pack2. This unofficial fan mod is not affiliated with Nexon. No third-party executable, personal profile, credentials or saved user settings are included.

For problems, report the exact location, game version, mod version and other installed camera/map mods.
