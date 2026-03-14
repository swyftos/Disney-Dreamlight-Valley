# DDV Dynamic Modifier v4.3

A MelonLoader mod for **Disney Dreamlight Valley** (IL2CPP Unity) that adds quality-of-life cheats with an in-game GUI menu.

**By Swyftos**

---

## Features

| Feature | Description |
|---------|-------------|
| **Free Purchase** | Buy anything without spending currency (Star Coins, Moonstones, StoreFront) |
| **Infinite Mana** | Actions that cost mana are free |
| **Pickup Multiplier** | Multiply the amount of items you pick up (x2 / x3 / x5 / x10) |
| **Game Speed** | Speed up the game while holding **Left Alt** (x2 / x3 / x5 / x10) |
| **Skip Cutscenes** | Automatically skips in-game cutscenes at startup |

All toggleable features are **OFF** by default. Toggle them from the in-game menu.

---

## Controls

| Key | Action |
|-----|--------|
| **F8** | Apply Harmony patches (must press first when in-game) |
| **INSERT** | Toggle the mod menu (GUI overlay) |
| **Left Alt** | Hold for game speed boost (when Game Speed is enabled) |

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
5. Press **INSERT** to open the mod menu and toggle features

---

## How It Works

The mod uses **Harmony patching** on IL2CPP methods at runtime. Patches are applied on demand (F8) to hook into game methods like `SpendCurrency`, `SpendMana`, `AddItem`, and more. An IMGUI-based overlay provides a toggle menu for each feature. Cutscene-skip patches are applied automatically at mod startup.

---

## Compatibility

- Game: Disney Dreamlight Valley (Steam)
- Framework: MelonLoader 0.6+
- Runtime: IL2CPP (net6.0)

---

## Troubleshooting

- **Patches not applying**: Make sure you're in-game (loaded save) before pressing F8. Check the MelonLoader console for error messages.
- **Menu not showing**: Press INSERT to toggle the GUI. Make sure patches were applied first with F8.
- **Game crashes**: Try enabling fewer features at a time. Check the MelonLoader console for details.
- **Other issues**: Please open an issue or make a pull request.

---

---

## Disclaimer

This mod is for **single-player / offline use only**. Use at your own risk. The authors are not responsible for any consequences of using this mod.

---

## Credits

- **Swyftos** - Mod author
- Based on research from [DDVMods](https://github.com/aedenthorn/DDVMods) BepInEx mods by aedenthorn
