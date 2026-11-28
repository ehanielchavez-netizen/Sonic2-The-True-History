# Changelog

All notable changes to **Sonic 2: The True History** are recorded here.

The project follows a simple release numbering scheme:
`MAJOR.MINOR` for public versions.

---

## [2.0] — 2026-11-28

### Fixes

- **Emerald Hill enemies restored:** removed the scripts that despawned Coconuts, Masher, Buzzer, Bee and Snail in Emerald Hill and the epilogue. All acts now keep their enemies, including the return from Hidden Palace.
- **Ocean Wind music fixed:** rebuilt `OceanWind.ogg` and `OceanWind_F.ogg` as clean OGG Vorbis files and forced playback when Ocean Wind loads.
- Kept the 1.5 route, the Genocide City Act 2 transition, the restored turrets and the Death Egg remix.
- Kept the 1.0 fixes: Genocide City layout, Act 1 layer crash fix, red springs, Act 2 goal post, Killerbug sprites and clean Cyber City music.
- Renamed the mod title to **Sonic 2: The True History**; the version now appears separately as **2.0** in the mod metadata.
- Base `Data/Game/GameConfig.bin` and `Scripts/LevelSelect/MenuControl.txt` remain untouched.

---

## [1.5] — 2026-11-27

### Campaign and transitions

- Corrected the route to match the final design:
  - **Warp Point 1:** end of Present (Metropolis Act 2) → Past.
  - **Past → Ruined Present:** direct, no Warp Point.
  - **Warp Point 2:** end of Ruined Present (Mystic Cave Act 2) → Future.
  - **Future → Last Battle:** direct, no Warp Point.
- **Genocide City Act 1 now leads into Act 2** before Last Battle; Act 2 is no longer skipped.
- **Hidden Palace** is now triggered by collecting the **7th Chaos Emerald**. After leaving it, the player returns to the **next zone**, not the same zone.
- Removed the old Hill Top → Hidden Palace route.

### Genocide City

- Restored the **Turret** objects in Genocide City Act 1 and Act 2 and kept the rest of the enemies.
- Kept the 1.0 fixes: Act 1 layer crash fix, red springs, Act 2 goal post and Killerbug sprite loading.
- Kept the clean Cyber City music replacement.

### Music

- Ocean Wind now uses the Enchanted Edition 1.5 theme.
- Genocide City now uses the Death Egg remix from Enchanted Edition 1.5; the final Death Egg music is unchanged.

### Versioning

- Renamed the release to **1.5** and updated the mod folder, in-game readmes and version fields.

---

## [1.0] — 2026-11-25

First public release.

### Campaign

- Rebuilt the campaign as a five-era time-travel route:
  Present → Past → Ruined Present → Future → Last Battle.
- Reordered the Level Select and era progression.
- Added the recovered zones to the main campaign:
  Ocean Wind, Jungle Woods, Sand Shower, Tropical Sun, Blue Ocean, Rock World
  and Genocide City.
- Kept Blue Ocean as a renamed Hydrocity, documented in the readmes.
- Kept the original Death Egg as the final level. No extra Death Egg, Gauntlet
  or all-boss arena was added.
- Added the Hidden Palace transition after the second Warp Point.
- Preserved the custom Warp Point 1 animated sequence.

### Genocide City

- Installed the Genocide City Act 1 layout from the GCZ source.
- Fixed the Act 1 background-layer configuration that could cause a
  divide-by-zero crash when the stage loaded.
- Removed the Genocide City Star Posts in 1.0 because of a checkpoint bug.
- Converted the yellow springs in Act 1 and Act 2 to red springs.
- Added a Sign Post to Act 2 so the act can be completed.
- Fixed Killerbug sprite loading for Genocide City.
- Removed the unused Killerbug Exhaust spawn that had no matching stage object.
- Replaced the corrupt Cyber City music file with a clean copy.

### Technical and presentation

- Fixed Warp Point 1 sprite-sheet removal paths.
- Restored the Warp Point 1 video playback path.
- Routed the second Warp Point to Hidden Palace (`stage.listPos = 35`).
- Updated the in-game English and Spanish readmes.
- Kept the base game's `Data/Game/GameConfig.bin` and
  `Scripts/LevelSelect/MenuControl.txt` untouched.
- Packaged the repository without the Sonic 2 Absolute base game or its
  original files.

### Known limitations in 1.0

- Blue Ocean is Hydrocity renamed, not a new level.
- Genocide City 2 is not included.
- Genocide City Act 2 uses the available GCZ source layout, not a completely
  original Act 2.
- Star Posts are disabled in Genocide City until the checkpoint bug is solved.
- Olympus and Madness Mountain are not fully playable.
- Some imported levels may differ visually or musically from their original
  releases.

---

## Unreleased / internal builds

Before 1.0, the mod went through private development and testing builds. Those
builds are not part of the public repository. Their fixes are summarized in the
1.0 notes above.

---

## Future

Planned work, if development continues:

- A full, original Genocide City Act 2.
- A proper checkpoint solution for Genocide City.
- Further cleanup of imported assets and credits.
- Compatibility testing with future Sonic 2 Absolute versions.

No release date is promised.
