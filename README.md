# Rai's Hidden Caches

An SPT BepInEx client mod that adds a flare-like smoke, light, and audio effect to all hidden caches scattered around the maps, making them easily visible.

Supports **SPT 4.0.13**.

---

## Features

- Smoke particle effect on every hidden cache
- Point light glow
- Looping audio
- Fully configurable via Configuration Manager (F12 in-game):
  - Toggle smoke, light, and audio independently
  - Customise the colour of the smoke and light

---

## Installation

1. Download the latest release from the [Releases](../../releases) page
2. Extract the zip into your SPT root folder (where `EscapeFromTarkov.exe` lives)
3. Confirm `BepInEx/plugins/RaiRai.HiddenCaches.dll` is present
4. Launch the game

---

## Building from source

### Prerequisites

- [.NET SDK](https://dotnet.microsoft.com/download) (net472)
- A working SPT 4.0.13 install

### Reference paths

The project uses absolute paths pointing to an SPT install at `C:\SPT\ModTest\`. If your install is elsewhere, update the `<HintPath>` entries in `RaiRai.HiddenCaches.csproj` to match your paths.

The following files are required:

| File | Source location in SPT install |
|------|-------------------------------|
| `BepInEx.dll` | `BepInEx\core\` |
| `0Harmony.dll` | `BepInEx\core\` |
| `spt-reflection.dll` | `BepInEx\plugins\spt\` |
| `Assembly-CSharp.dll` | `EscapeFromTarkov_Data\Managed\` |
| `Comfort.dll` | `EscapeFromTarkov_Data\Managed\` |
| `UnityEngine.dll` | `EscapeFromTarkov_Data\Managed\` |
| `UnityEngine.AudioModule.dll` | `EscapeFromTarkov_Data\Managed\` |
| `UnityEngine.CoreModule.dll` | `EscapeFromTarkov_Data\Managed\` |
| `UnityEngine.IMGUIModule.dll` | `EscapeFromTarkov_Data\Managed\` |
| `UnityEngine.ParticleSystemModule.dll` | `EscapeFromTarkov_Data\Managed\` |

### Steps

1. Clone the repository
2. Update `<HintPath>` entries in `RaiRai.HiddenCaches.csproj` if your SPT install path differs
3. Build in Release configuration
4. Copy `build/plugins/RaiRai.HiddenCaches.dll` to `BepInEx/plugins/` in your SPT install

---

## Credits

- **RaiRaiTheRaichu** — original mod
- **Terkoiz** — contributions
- **VonBraunZ** — 4.0.13 port
