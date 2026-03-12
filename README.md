# DDV Dynamic Modifier - MelonLoader Mod

A MelonLoader mod for **Disney Dreamlight Valley** (IL2CPP Unity) that adds quality-of-life cheats. All features are toggled independently via hotkeys.

**By Swyftos**

---

## Features

| Hotkey | Feature | Description |
|--------|---------|-------------|
| **F8** | Apply Patches | Must be pressed first when in-game to activate the mod |
| **F2** | Free Purchase | Buy anything without spending currency (Star Coins / Moonstones) |
| **F3** | Infinite Mana | Actions that cost mana are free |
| **F4** | Pickup Multiplier | Multiply the amount of items you pick up |
| **F5** | Cycle Multiplier | Cycle through x2 / x3 / x5 / x10 |
| **F6** | Instant Grow | Crops and trees grow instantly (experimental) |
| **F7** | Sprint | Hold **Left Alt** while moving to run 3x faster |

All features are **OFF** by default after patching. Toggle them individually with the hotkeys above.

---

## Installation

### Requirements
- [MelonLoader](https://melonwiki.xyz/) installed for Disney Dreamlight Valley
  - Download MelonLoader Installer from [GitHub](https://github.com/LavaGang/MelonLoader/releases)
  - Point it at your game executable: `Disney Dreamlight Valley.exe`

### Install the Mod
1. Download `DDVModifier.dll` from the [Releases](Releases/) folder
2. Copy it to your game's `Mods` folder:
   ```
   <Steam>/steamapps/common/Disney Dreamlight Valley/Mods/DDVModifier.dll
   ```
3. Launch the game
4. Once in-game (after loading your save), press **F8** to apply patches
5. Use the hotkeys above to toggle features

---

## How It Works

The mod uses **Harmony patching** on IL2CPP methods at runtime:

## Compatibility

- Game: Disney Dreamlight Valley (Steam)
- Framework: MelonLoader 0.6+
- Runtime: IL2CPP (net6.0)

---

## Troubleshooting

- **Patches not applying**: Make sure you're in-game (loaded save) before pressing F8. Check the MelonLoader console for error messages.
- **Features not working after F8**: Toggle them with their respective hotkeys (F2-F7). They start OFF by default.
- **Game crashes**: Try enabling fewer features at a time. Disable Instant Grow first as it's experimental.
- **Other please make a pull request**

---

## Disclaimer

This mod is for **single-player / offline use only**. Use at your own risk. The authors are not responsible for any consequences of using this mod.

---

## Credits

- **Swyftos** - Mod author
- Based on research from [DDVMods](https://github.com/aedenthorn/DDVMods) BepInEx mods by aedenthorn
