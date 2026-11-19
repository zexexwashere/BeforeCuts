# Before Cuts 🎬
> High-Performance AI Scenepack & Shot Cut Studio for Video Editors

**Before Cuts** is a modern, standalone Windows desktop application built to turn movies, anime, and raw footage into clean, frame-accurate scenepacks and cut clips in seconds using neural AI.

Designed specifically for video editors, AMV/edit creators, and VFX artists who need fast, zero-latency timeline scrubbing, intelligent scene detection, and instant integration with Adobe After Effects.

---

## ✨ Features

- **🤖 Neural AI Shot Detection**: Built-in TransNet V2 neural engine powered by DirectML GPU acceleration to detect scene changes automatically without manual blade work.
- **⚡ Zero-Latency Scrubbing**: Instantaneous timeline scrubbing across multi-gigabyte 4K and 1080p files with zero lag or buffering.
- **🎯 In & Out Range Trimming**: Mark custom In `[I]` and Out `[O]` boundaries to process specific sections or analyze full-length movies.
- **🖼️ Interactive Clips Gallery**: Visual card grid of all detected scenes with auto-generated thumbnails, single-click loop audition, and frame nudging (`-1f` / `+1f`).
- **📦 Dual Export Options**:
  - **Single Video**: Automatically stitches all selected scenes into one clean scenepack file.
  - **Individual Clips**: Slices each selected scene into numbered clips (`clip_001.mp4`, etc.).
  - **Encoding Choices**: Lossless stream copy (`-c copy`) for instant exports or Frame-Accurate x264 renders.
- **💾 Native Project Files (`.bcp`)**: Save your timeline sessions and cut selections into lightweight `.bcp` project files.
- **🔌 Adobe After Effects Extension**: Included CEP extension allows you to import `.cuts` metadata directly into After Effects to automatically slice composition layers in a single click.
- **🎨 Sleek Dark Glass UI**: Apple-inspired dark midnight sapphire aesthetic with customizable accent hues and full-screen workspace mode.

---

## 📥 Download & Installation

1. Go to the **[Releases](https://github.com/zexexwashere/BeforeCuts/releases)** section of this repository.
2. Download the latest installer: **`BeforeCuts_Setup.exe`**.
3. Run the installer and follow the setup wizard:
   - ✅ Optionally creates a clean Desktop shortcut.
   - ✅ Automatically registers `.bcp` and `.cuts` file associations.
   - ✅ Automatically installs the Adobe After Effects extension if After Effects is detected.
4. Launch **Before Cuts** from the Start Menu or Desktop!

---

## 🚀 Quick Start

1. **Import Footage**: Drag and drop any video file directly into Before Cuts (or press `Ctrl+O`).
2. **Scan Scenes**: Press **Detect Scenes** to run AI scene cut analysis (or set `[I]` and `[O]` points to scan a specific segment).
3. **Review & Pick**: Click any thumbnail in the gallery to preview that scene on loop. Select or deselect clips to customize your scenepack.
4. **Export**:
   - Click **Export Scenepack** (`Ctrl+E`) to render your video, or
   - Export `.cuts` data to split layers automatically inside Adobe After Effects!

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| **`Space`** | Play / Pause video |
| **`Left` / `Right`** | Step 1 frame backward / forward |
| **`Shift` + `Left` / `Right`** | Step 1 second backward / forward |
| **`I`** | Set In marker at playhead |
| **`O`** | Set Out marker at playhead |
| **`F11` / `F`** | **Toggle Fullscreen Mode** |
| **`Ctrl` + `S`** | Save Project (`.bcp`) |
| **`Ctrl` + `Shift` + `S`** | Save Project As... |
| **`Ctrl` + `O`** | Open Project File |
| **`Ctrl` + `E`** | Open Scenepack Exporter |
| **`Ctrl` + `Z`** | Undo cut selection |
| **`Ctrl` + `Y`** | Redo cut selection |
| **`V`** | Toggle Footage / Videos Bin |
| **`M`** | Toggle Audio Mute |
| **`Esc`** | Exit Scene Loop Preview / Close Dialogs |

---

## 💻 System Requirements

- **Operating System**: Windows 10 or Windows 11 (64-bit)
- **GPU**: Any DirectX 12 compatible GPU (NVIDIA, AMD, or Intel) for hardware-accelerated AI detection; CPU fallback supported.
- **Storage**: ~300 MB free disk space for the application and AI neural model.

---

## ⚖️ License & Notice

**Before Cuts** is developed by **Zexex**. All rights reserved (Proprietary / Closed Source).

*Disclaimer: Before Cuts is an independent desktop application and is not affiliated with, endorsed by, or sponsored by Adobe Inc. Adobe and Adobe After Effects are registered trademarks of Adobe Inc.*
