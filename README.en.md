# Sephiria Endless Trial

[한국어](README.md) | [English](README.en.md) | [日本語](README.ja.md) | [简体中文](README.zh-CN.md)

**Endless Trial** is an unofficial trial mod for Sephiria. Fight through stages in a separate trial arena and visit a merchant and reward room every five stages.

The download and installation instructions below are for the Windows Steam version. [v1.0.0 release notes (Korean)](RELEASE_NOTES_v1.0.0.md)

## Download and installation

1. Download **`Endless_Trial.zip`** from the [latest release](https://github.com/TaeHyun015/Sephiria_Endless_Trial/releases/latest).
2. Close the game completely.
3. Extract the ZIP into the `AddOns` directory in your Sephiria installation. The resulting layout should be:

   ```text
   Sephiria/
   └─ AddOns/
      └─ Endless_Trial/
         ├─ Endless_Trial.dll
         ├─ endless_trial_floor
         ├─ metadata.json
         └─ Endless_Trial/
            └─ trial_bg.png
   ```

4. Start the game. To update an existing installation manually, close the game and extract the new ZIP to the same location, replacing the old files.

The ZIP already contains an `Endless_Trial` folder. Extract it into `AddOns`, not into `AddOns/Endless_Trial`, to avoid an extra nested folder.

## How to play

- At the trial entrance portal in the multiplayer zone, the host selects a save slot to enter. In multiplayer, all players must gather near the entrance.
- Start a stage at the trial stone tablet. The ending credits music plays in the trial arena while a stage is in progress.
- Every five stages, a portal opens to the merchant and reward room. All players must return to the battle arena before the next stage can begin.
- Use the save and return portal to save your progress and leave. There are three trial save slots; in multiplayer, the host manages the save.

## Automatic updates

When a new version is published, an update prompt appears when the game starts. If you accept, the mod downloads the release's `Endless_Trial.zip`, checks its SHA256 hash, replaces the mod files after the game closes, and restarts the game. If you decline, you can continue playing with the installed version.

For automatic updates to detect a release, it must be **Published**, and its tag must match `modVersion` in the ZIP's `metadata.json`. The release asset must be named exactly `Endless_Trial.zip`. A release with the same version as the installed mod will not trigger an update.

Trial save files are not included in the ZIP in the mod installation folder. Do not include save files in an update ZIP. Back up important save data before reinstalling the game or mod.

## Troubleshooting

- **The mod does not appear:** Check the folder layout above and make sure `metadata.json`, the DLL, and `endless_trial_floor` are present.
- **No automatic update prompt appears:** Check that the new release tag is newer than the installed version, that the release is neither a Draft nor a Prerelease, and that the ZIP filename is correct.
- **Reporting a bug:** Include the game version, mod version, steps to reproduce, and relevant lines from `C:\Users\<username>\AppData\LocalLow\TEAMHORAY\Sephiria\Player.log`. Review the log for personal information before sharing it publicly.

## License and rights

This mod is not an official TEAM HORAY product. The rights to the Sephiria name, original game assets, and music belong to their respective owners. Distributing this mod does not grant separate permission to reuse those original materials.

This repository currently does not specify an open source license for reusing the mod code. Publicly available source code without a license should not be assumed to permit modification or redistribution. An open source license for the mod code may be decided separately.
