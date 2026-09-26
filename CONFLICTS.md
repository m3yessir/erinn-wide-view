# Findias / Uiscias file conflicts

Audit date: **2026-09-26**. Compared all 175 release paths against the `usedFiles` declarations of all 122 variants in 100 groups in the [Uiscias v1.65.0 catalog](https://github.com/Root50199/Uiscias/releases/download/v1.65.0/manifestCatalog.json), generated 2026-09-25T16:12:38.439Z. Paths were compared case-insensitively with normalized directory separators. Every variant had a file list.

Result: **12 variants in six groups overlap**. These are catalog-declared whole-file collisions, not observed in-game failures for every combination. The other 110 variants have no declared direct overlap, which is not a guarantee of compatibility. Future releases and mods outside this catalog are not covered.

Disable overlapping packages or use a deliberately merged compatibility build. Do not rely on filename order or assume that Findias detects this manually installed package. Wide View does not include the zoom extensions, decluttering, or gameplay fixes from these mods. Even Farm WASD Bug Fix No FoV replaces a shared file.

## Bri Leith Zoom And FoV

| Affected variant | Archive filename |
| --- | --- |
| Bri Leith Zoom And FoV60 | `UisciasBriLeithZoomAndFoV60_00004.it` |
| Bri Leith Zoom And FoV90 | `UisciasBriLeithZoomAndFoV90_00004.it` |

Shared paths in each listed variant:

- `data/world/MRD_1S/MRD_1S.rgn`
- `data/world/MRD_2S/MRD_2S.rgn`
- `data/world/MRD_3S/MRD_3S.rgn`
- `data/world/MRD/MRD.rgn`

## Crom Bas Zoom And FoV And Declutter

| Affected variant | Archive filename |
| --- | --- |
| Crom Bas Zoom And FoV And Declutter 60 FoV | `UisciasCromBasZoomAndFoVAndDeclutter60FoV_00003.it` |
| Crom Bas Zoom And FoV And Declutter 90 FoV | `UisciasCromBasZoomAndFoVAndDeclutter90FoV_00003.it` |

Shared paths in each listed variant:

- `data/world/PDG_dungeon_A/PDG_dungeon_A.rgn`
- `data/world/PDG_dungeon_B/PDG_dungeon_B.rgn`
- `data/world/TR_main_field_01/TR_main_field_01.rgn`

## Farm WASD Bug Fix

| Affected variant | Archive filename |
| --- | --- |
| Farm WASD Bug Fix 90 FoV | `UisciasFarmWASDBugFix90Fov_00001.it` |
| Farm WASD Bug Fix No FoV | `UisciasFarmWASDBugFixNoFoV_00001.it` |

Shared paths in each listed variant:

- `data/world/Taillteann_NewFarm/Taillteann_NewFarm.rgn`

## Glenn Bearna Zoom

| Affected variant | Archive filename |
| --- | --- |
| Glenn Bearna Zoom FoV 60 | `UisciasGlennBearnaZoomAndFoV60_00001.it` |
| Glenn Bearna Zoom FoV 60 With Declutter | `UisciasGlennBearnaZoomAndFoV60WithDeclutter_00001.it` |
| Glenn Bearna Zoom FoV 90 | `UisciasGlennBearnaZoomAndFoV90_00001.it` |
| Glenn Bearna Zoom FoV 90 With Declutter | `UisciasGlennBearnaZoomAndFoV90WithDeclutter_00001.it` |

Shared paths in each listed variant:

- `data/world/Glenn_Bearna_boss_dungeon01_day/Glenn_Bearna_boss_dungeon01_day.rgn`
- `data/world/Glenn_Bearna_boss_dungeon01_night/Glenn_Bearna_boss_dungeon01_night.rgn`
- `data/world/Glenn_Bearna_dungeon_day/Glenn_Bearna_dungeon_day.rgn`
- `data/world/Glenn_Bearna_dungeon01_night/Glenn_Bearna_dungeon01_night.rgn`

## Homestead Zoom And FoV

| Affected variant | Archive filename |
| --- | --- |
| Homestead Zoom And FoV | `UisciasHomesteadZoomAndFoV_00001.it` |

Shared paths in each listed variant:

- `data/world/Farm_Grassland_90/Farm_Grassland_90.rgn`

## Moonlight Island Zoom And FoV

| Affected variant | Archive filename |
| --- | --- |
| Moonlight Island Zoom And FoV | `UisciasMoonlightIslandZoomAndFoV_00003.it` |

Shared paths in each listed variant:

- `data/world/Private_Island_152/Private_Island_152.rgn`
