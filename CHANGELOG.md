# Changelog

## v0.3.0-beta — 2026-09-30

Adds 254 fixed interior region files and 63 room variants, matching the tested expanded Mooncrest FOV payload. All 176 previous region payloads are unchanged. Total: 493 files at fixed 110 FOV. Adds Dungeon Statue Fix and Phantasm Zoom And Delag to the conflict list. Generated dungeon floors remain unsupported.

## 0.2.0-beta — 2026-09-26

- Bundles the existing outdoor 110 FOV mod and the working Crom Bás 110 FOV add-on into one package.
- Adds NTD_dungeon.rgn, bringing the total to 176 region files. All 175 previous outdoor files are unchanged.
- Keeps the Sidhe visibility/fog experiment separate.
- Updates the conflict details to include the Crom Bás dungeon region.
- Upgrade: remove the old Wide View package and the separate Crom Bás add-on before installing m3yessirErinnWideView110_00002.it.
- Archive contents verified against both input packages; combined runtime testing is still pending. The author reported the Crom Bás test working without specifying every difficulty or boss room.

## 0.1.0-beta — 2026-09-26

- First branded standalone release by m3yessir.
- Requests FOV 110 in 175 supported outdoor region files/templates.
- Uses stock game regions and preserves their original zoom limits.
- Excludes interior overrides after black rendering was reported in Tir Chonaill shops.
- Excludes generated-dungeon and mission-variation camera changes.
- Removes the unrelated Uiscias mods included in earlier personal test packages.
- Documents file overlaps with 12 variants across six Findias/Uiscias mod groups, based on the v1.65.0 catalog audit. Documentation update only; the `.it` package is unchanged.

This standalone release is separate from personal test versions `CustomErinnFov110_00001.it` and `CustomErinnFov110_00002.it`; those are not public release versions.
