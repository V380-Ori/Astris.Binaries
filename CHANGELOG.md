# 1.0.30+115dc1ae0
Improvements:
- Implement game library cache to improve scanning time for external drives.
- Add an option `Always use immediate presentation` to allow disabling host V-Sync which reduces presentation delay at the cost of possible screen tearing.
- Support adding game updates/DLCs/mods by drag and drop in game library.

Fixes:
- Workaround `BioShock Remastered` being stuck on a black screen during launch.
- Fix a regression causing some games such as `Mario Party Superstars` to crash by being unable to access save data.
- Fix a regression causing a crash during quest loading in `Monster Hunter Rise: Sunbreak`.

# 1.0.29+835d74ccc
Fixes:
- Fix a regression causing toolbar items to always use dark mode color scheme.

# 1.0.28+76715232a
Fixes:
- Fix crash in `The Lego Ninjago Movie Video Game` during launch.

# 1.0.27+e70414f92
Improvements:
- Add an option to allow background controller input (disabled by default).

Fixes:
- Fix a regression causing graphical issue in `Donkey Kong Country: Tropical Freeze`.
- Fix crash in `Hades II` during loading/entering specific areas.
- Fix behavior of `Auto-hide interface` option.

# 1.0.26+3acc192af
Fixes:
- Fix a regression causing `Bayonetta 3` and `Pokémon Legends: Arceus` to crash.

# 1.0.25+66283e026
Improvements:
- Add support for [NSZ](https://github.com/nicoboss/nsz) zstd-compressed NCA/NSP/XCI.
    - NOTE: Only block compression is supported.

Fixes:
- Fix `Metal Gear Solid 4: Guns of the Patriots - Master Collection Version` crash.

Vulkan Translation Layers:
- Update KosmicKrisp, based on [97bfc0f8](https://gitlab.freedesktop.org/mesa/mesa/-/commit/97bfc0f88f43554b47f05ad37512f98cd086a80d) + non-Metal-4-related command encoder upstream changes.

# 1.0.24+da061dba2
Fixes:
- Fix performance regression in some Unreal Engine 4/5 titles such as `Stray`.
- Workaround `Absolum` crash when using `1.2.0` game version.
- An attempt to fix play time sometimes not saving after a session.

# 1.0.23+46883fa0b
Improvements:
- Game Overlay (macOS 26+):
    - Add all graphical enhancements options.
    - Any changed graphical option now overrides global option and can be restored (right-click).

Fixes:
- Fix possible out-of-memory system crash when using MoltenVK.
- Fix already connected controller input not working if app is launched via LaunchServices (Finder/Spotlight/ES-DE) requiring to reconnect controller.
- Fix `Marvel Cosmic Invasion` crash during launch.
- Fix `TIEBREAK+: Official Game of the ATP and WTA` crash during launch.
- Fix `Pokémon Let's Go Pikachu` crash that happens depending on the number of scene transitions and encounters.
- Workaround `KAMEN RIDER CLIMAX SCRAMBLE` crash during launch.

Vulkan Translation Layers:
- Update KosmicKrisp, based on [97bfc0f8](https://gitlab.freedesktop.org/mesa/mesa/-/commit/97bfc0f88f43554b47f05ad37512f98cd086a80d) + non-Metal-4-related command encoder upstream changes.
- Update MoltenVK to [1.4.3-preview.6](https://github.com/V380-Ori/Ryujinx.MoltenVK/commit/45f9b641e45f1d150f3521d74808477add9e975b).

# 1.0.22+d354de498
Fixes:
- Fix graphical issue in `The Legend of Zelda: Tears of the Kingdom` when not using 1x resolution scaling.
- Fix graphical issue in `Game Builder Garage`.
- Fix crash in `Kirby's Return to DreamLand Deluxe` after completing a level.

Vulkan Translation Layers:
- Update MoltenVK to [1.4.3-preview.4](https://github.com/V380-Ori/Ryujinx.MoltenVK/commit/fbe2476fc611ba274f3e3208c759c2990c73def6).

# 1.0.21+83437d20e
Fixes:
- Fix `Yooka-Laylee` crash on launch.
- Fix performance regression on MoltenVK in some games such as `Monster Hunter Rise: Sunbreak`.

Vulkan Translation Layers:
- Update MoltenVK to [1.4.3-preview.3](https://github.com/V380-Ori/Ryujinx.MoltenVK/commit/8a8f8f7231ea8a47bbf5db55033fa7717c44dd9e).

# 1.0.20+141efefc5
Fixes:
- Fix a possible crash during emulation start.

# 1.0.19+f87bcdbca
Fixes:
- Fix a possible crash after exiting full screen on macOS 26+.

# 1.0.18+24bfd57a8
Fixes:
- Fix incorrect controller triggers threshold logic.

# 1.0.17+ac97c0890
Improvements:
- Implement keyboard input mapping.
- Add controller sticks deadzone & triggers threshold options.
- Edge-to-edge window during emulation with locked aspect ratio & new game overlay. (macOS 26+)
- Add docked mode & v-sync toggles to the menu for keyboard shortcuts during emulation.

Fixes:
- Fix `Rhythm Heaven Groove` infinite loading.
- Fix an issue where incorrect avatar image size for user profiles was set after creating/editing profile which caused crashes in some games.
    - Note: If you made any changes to user profiles, you will have to choose an avatar image for the profile again to resolve this issue.
- Do not show duplicate games in game library, and prioritize by internal volume.
- Fix an issue where pressing ESC during emulation wouldn't exit full screen.

Vulkan Translation Layers:
- Update MoltenVK to [1.4.3-preview.1](https://github.com/V380-Ori/Ryujinx.MoltenVK/commit/f16a46efd19e0ec690a801118bacb4e461be9c06).
- Update KosmicKrisp to [3e2d8517](https://gitlab.freedesktop.org/mesa/mesa/-/commit/3e2d8517b897026377267c09975db83525d2fc95).

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
