# DDV Dynamic Modifier v4.5

A MelonLoader mod for **Disney Dreamlight Valley** (IL2CPP Unity) that adds quality-of-life cheats with an in-game GUI menu.

**By Swyftos**

---

## Features

| Feature | Description |
|---------|-------------|
| **Free Purchase** | Buy anything without spending currency (Star Coins, Moonstones, StoreFront) |
| **Infinite Mana** | All mana costs are zero |
| **Free Crafting** | Craft any recipe without needing ingredients |
| **Pickup Multiplier** | Multiply item pickups (x2 / x3 / x5 / x10) |
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

## Screenshots

The mod features a dark-themed in-game overlay with pill-shaped toggles, organized by category (Economy, Multipliers, Gameplay).

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

The mod uses **Harmony patching** on IL2CPP methods at runtime:

- **Economy patches** hook into `SpendCurrency`, `SpendMana`, `HasEnoughCurrency`, `SpendStoreFrontSpecificCurrency` and more
- **Free Crafting** patches `TryConsumeIngredients`, `GetMissingIngredientCount`, `GetMaxCraftable` on `CraftWithRecipe`
- **Pickup Multiplier** intercepts `ContainerInventory.AddItem` using `__originalMethod.Invoke` with modified amounts
- **Skip Cutscenes** patches `DebugSettings` getters at mod startup (no keybind needed)

An IMGUI-based overlay provides a toggle menu for each feature.

---

## Compatibility

- Game: Disney Dreamlight Valley (Steam)
- Framework: MelonLoader 0.6+
- Runtime: IL2CPP (net6.0)

---

## Troubleshooting

- **Patches not applying**: Make sure you're in-game (loaded save) before pressing F8. Check the MelonLoader console for error messages.
- **Menu not showing**: Press INSERT to toggle the GUI. Make sure patches were applied first with F8.
- **Free Crafting not working**: Make sure you toggle it ON in the menu after pressing F8. Note: while enabled, item removal is blocked (disable it when not crafting).
- **Game crashes**: Try enabling fewer features at a time. Check the MelonLoader console for details.
- **Other issues**: Please open an issue or make a pull request.

---

## Changelog

See [RELEASE_NOTES.md](RELEASE_NOTES.md) for full version history.

---

## Disclaimer

This mod is for **single-player / offline use only**. Use at your own risk. The authors are not responsible for any consequences of using this mod.

---

## Credits

- **Swyftos** - Mod author
- Based on research from [DDVMods](https://github.com/aedenthorn/DDVMods) BepInEx mods by aedenthorn
