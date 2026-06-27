# 1.0.16+0e933ae41
Improvements:
- Add profile selection to the toolbar to quickly switch between user profiles.

Fixes:
- Fix an issue where "Add Profile..." button was missing in settings if the user had only one profile.

# 1.0.15+89e095356
Breaking change:
- macOS 15.0 is now the minimum supported version.

Improvements:
- Whole UI project refinements:
    - New settings to match modern macOS.
    - Improvements to readability & accessibility.
- Support combo XCI games for auto-selection of updates/DLCs during library scanning.

Fixes:
- Fix a possible crash caused by data race during library scanning.
- Fix an issue where some library folders couldn’t be removed.
- Prevent eviction of library folders located on disconnected external storage.

# 1.0.14+04b3b13a8
Fixes:
- Fix a regression causing captured frames (screenshots) to be saved with incorrect transparency.

# 1.0.13+03a1656fe
Improvements:
- Implement filesystem reactive game library.
- Improve automatic game updates & DLCs selection.
- Add option to hide game overlay.

Fixes:
- Fix a regression causing missing graphics in `Pokemon Legends: Arceus` and `The Legend of Zelda: Echoes of Wisdom`.

Vulkan Translation Layers:
- Update KosmicKrisp to [e8ab81cc](https://gitlab.freedesktop.org/mesa/mesa/-/commit/e8ab81cc3a1c35090e1534f356b8315456ba91a9).

# 1.0.12+1f3919be0
Fixes:
- Fix a regression causing missing graphics in `Luigi's Mansion 3`.
- Fix a regression causing graphical glitches in `Metroid Prime Remastered`.

# 1.0.11+c2c7ba1a7
Fixes:
- Fix crash on launch when using macOS 14.

# 1.0.10+c349d3e44
Improvements:
- Initial support for 22.0.0 titles.
- Show an alert when an emulated game's file system integrity verification hash mismatches, allowing the user to continue emulation instead of crashing.
- More options in per-game settings.

Fixes:
- Fix controller gyroscope calibration.
- Fix an issue where debugging tools are unable to attach to the Astris process.
