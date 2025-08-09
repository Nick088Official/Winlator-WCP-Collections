# Winlator WCP Collections

This repository is a curated list of collections of pre-packaged `.wcp` files for the Winlator Android emulator. All packages are generated using the tools from the [Winlator-WCP-Toolkit](https://github.com/Nick088Official/Winlator-WCP-Toolkit) project.

## What is `.wcp`?

.wcp is the file extension for add-ons. It is compressed using XZ or Zstd and includes a profile.json file as a manifest. You can create your own add-on files containing various contents. Since these files often include executable programs, make sure to verify that add-ons from other sources do not contain malicious software before installation.

## How to Find and Download `.wcp` Files?

All packages are organized into "Collection Releases." This means there is a single, living release for each category that is continuously updated with new versions.

**Click the link below to go directly to the Releases page:**

## -> [View All WCP Collections Here](https://github.com/Nick088Official/Winlator-WCP-Collections/releases) <-

On the releases page, you will find collections like:
-   **DXVK (Official) Collection**
-   **DXVK-Sarek Collection**
-   **DXVK GPLAsync Collection**
-   **vkd3d-proton Collection**
-   **FEXCore Collection**

Simply find the collection you need. All downloadable `.wcp` files are in the "Assets" section of that release.

### Install the `.wcp` files on:

#### Winlator Cmod (Bionic)

1.  Get the latest release of [Winlator Cmod (Bionic)](https://github.com/coffincolors/winlator/releases)
2.  Get the `.wcp` files.
3.  Open Winlator Cmod (Bionic) on your phone.
4.  Navigate to "Contents", and choose which type to install.
5.  Tap the "Install Comntent" button.
6.  Select your `.wcp` file from the file picker. It will be installed soon.
7.  The new component will now be available to select for your containers!


---

### Choosing the Right DXVK Version

| DXVK Version | Primary Purpose | Best For... | Potential Downsides |
| :--- | :--- | :--- | :--- |
| **Official DXVK** | The standard, stable version. | **Most users.** This should always be your starting point. | Can have noticeable stutter the first time a new effect or area is shown in-game. |
| **Nightly/Dev Builds** | The absolute latest, unreleased code with bleeding-edge fixes. | Testing a fix for a specific game that is broken on the stable release. | Potentially unstable and may introduce new bugs. Use for troubleshooting only. |
| **DXVK-Async** | Reduces stutter by compiling shaders on a background thread. | Games with heavy, constant stutter (e.g., Unreal Engine games). | Can cause graphical glitches or pop-in as it's technically a "hack". Less common now. |
| **DXVK-GPLAsync** | Modern, more efficient stutter reduction using a proper Vulkan extension. | A more stable alternative to regular Async on supported drivers. | Requires newer drivers that support the `VK_EXT_graphics_pipeline_library` extension. |
| **DXVK-Sarek** | Backports new game fixes to an older DXVK base for maximum compatibility. | **Mali & SD8 Elite users**, Users with older hardware/drivers that don't support modern Vulkan features. | Lacks the latest performance optimizations from the newest official DXVK versions. |

#### Detailed Explanations

-   **Official DXVK:** This is the baseline. When a game needs to show a new visual effect, it has to compile a "shader" for your GPU. This can cause a brief pause or "stutter." Official DXVK does this as needed, so you might see stutter the first time you play through an area.

-   **DXVK-Async:** This is the classic "stutter fix." It moves that shader compilation to a separate, parallel thread. The game doesn't have to wait for it, which makes gameplay feel smoother. However, because the game doesn't wait, a shader might not be ready in time, causing visual glitches like textures popping in late or flickering objects.

-   **DXVK-GPLAsync:** This is the modern successor to Async. It uses an official Vulkan feature (`Graphics Pipeline Library`) that is designed for this exact purpose. It's much more stable and less "hacky" than the original Async, resulting in fewer visual bugs while still reducing stutter. **If your device supports it, this is generally better than the old Async.**

-   **DXVK-Sarek:** Think of this as a Long-Term Support (LTS) version with benefits. It sticks with an older, very compatible DXVK version (like 1.10.3) that works on a wide range of hardware and then adds specific, targeted fixes for newer games. It prioritizes "it runs" over "it runs at the absolute maximum possible FPS." **Suggested for not much supported hardware, such as SD8 Elite & Mali**

---

## Licensing

This project follows a two-tier licensing system to respect all creators' work.

1.  **This Repository:** The original content of this repository (this `README.md`, etc.) is licensed under the **MIT License**. You can find it in the `LICENSE` file in the root directory.
2.  **The WCP Files:** Each `.wcp` file is a redistribution derivative work of another project's work and is governed by its **original open-source license**. To comply with these licenses, a full copy of each component's license is permanently available in the **[LICENSES/](https://github.com/Nick088Official/Winlator-WCP-Collections/tree/main/LICENSES)** folder of this repository.

By downloading and using a `.wcp` file, you agree to the terms of its original license.
