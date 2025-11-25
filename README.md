# 📻 Custom Boombox Sound Mod

## Project Overview

This project is a client-side mod developed for Lethal Company using the BepInEx framework. It utilizes runtime patching (Harmony) to intercept the game's audio logic and replace the default boombox music with custom, user-defined audio files dynamically.

## Key Features

* **Runtime Asset Replacement:** Intercepts game calls to swap audio clips in real-time without modifying base game files.
* **Custom Audio Support:** Users can easily inject their own `.ogg` files.
* **Royalty-Free Default:** Comes pre-packaged with a royalty-free track ("Susan - 125 bpm") ensuring stream-safe usage.

## Technical Stack

* **Language:** C#
* **Framework:** .NET Framework 4.7.2
* **Modding Tools:** BepInEx 5.x, Harmony (0Harmony)
* **Engine:** Unity (Runtime Patching)

---

## 🛠️ How to Build (Compile)

To compile this plugin from the source code, follow these steps to ensure dependencies are resolved correctly.

### 1. Requirements

* **.NET Framework 4.7.2 Developer Pack**
* **Visual Studio 2019** or later
* **BepInEx 5.x**
* **Game Installation:** You must have the game installed locally to reference its DLLs (`Assembly-CSharp.dll`, `UnityEngine.dll`, etc.).

### 2. Folder Structure

Ensure your project directory is organized as follows for the `.csproj` file to locate files correctly:

```text
CustomBoomboxSound/
├── CustomBoomboxSound.csproj   # Main project configuration
├── Plugin.cs                   # C# Source code containing patches
└── custom.ogg                  # Audio file (optional, for testing)
