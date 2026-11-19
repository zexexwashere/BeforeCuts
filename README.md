# Before Cuts 🎬
> High-Performance AI Scene Detection & Video Cut Studio

**Before Cuts** is a fast, lightweight Windows desktop application designed for video editors, AMV/edit creators, and VFX artists to turn movies, anime, and long raw footage into clean, frame-accurate scenepacks in seconds.

Powered by the **TransNet V2** neural network and **DirectML GPU acceleration**, Before Cuts automatically detects cut points with zero manual blade work, supports instant timeline scrubbing, and seamlessly integrates with **Adobe After Effects**.

---

## ⚡ Key Features

### 🤖 AI & Manual Scene Detection
- **TransNet V2 Neural Engine**: GPU-accelerated cut detection via DirectML (DirectX 12) with CPU fallback.
- **Sensitivity Modes**: Choose between *Balanced*, *Aggressive* (more cuts), *Conservative* (fewer cuts), or set a custom threshold.
- **Min Frame Filter**: Prevent micro-cuts and flashing frames (configurable, default 6 frames).
- **Manual Cut**: Slice instantly at the current playhead at any time.

### ⏱️ Zero-Latency Player & Precision Scrubbing
- **Instant Scrubbing**: Smooth scrubbing across large 1080p and 4K video files without buffering.
- **In & Out Markers**: Restrict AI analysis or playback to a specific segment using `[I]` and `[O]`.
- **Work Area Snapping**: Drag the selection range or handles; hold `Shift` to snap to playhead, start, or end.
- **Frame-Accurate Timecode Editor**: Click any timecode to nudge frames (`-10f`, `-1f`, `+1f`, `+10f`) or jump to extremes.
- **Playback Speeds**: Cycle through 0.25x, 0.5x, 1x, 1.5x, and 2x speed.
- **Audio Mute**: Instant audio toggle (`M`).

### 🎞️ Cuts Manager & Isolated Preview
- **Interactive Thumbnails**: Every cut generates a preview card with duration and frame stats.
- **Isolated Cut Preview**: Click any cut card to audition and loop *only* that scene. Press `Esc` to return to the full timeline.
- **Batch Tools**: `Select All`, `Unselect All`, and `Remove Unselected` to keep your workspace clean.
- **Filter Tabs**: View cuts from `All` loaded videos or only the `Current Video`.

### 📂 Multi-Video Media Bin
- **Drag & Drop Import**: Drop video files directly onto the app window.
- **Footage Inspector**: View resolution, frame rate, audio channels, codec, and bitrate in a single click.
- **Quick Replace**: Swap video files while preserving existing cut points.

### 📦 Export Options
- **Merged Scenepack**: Stitches all selected cuts into a single master video file.
- **Individual Clips**: Slices each cut into separate numbered files (`clip_001.mp4`, etc.).
- **Lossless Stream Copy (`-c copy`)**: Exports in seconds with zero quality loss and no re-encoding.
- **Custom x264 Render**: Encode with custom CRF quality, presets, resolution scaling, and custom FPS.
- **After Effects Data (`.cuts`)**: Export cut timestamps for instant layer splitting in After Effects.

### 🔌 Adobe After Effects Integration
- Includes a dedicated **CEP Extension** (`com.zexex.beforecuts`).
- Load any `.cuts` file inside After Effects to automatically split your composition layers at the exact cut frames in one click.

### ⚙️ Built-in Engine & Model Manager
- **FFmpeg (`C:\ffmpeg`)**: Built-in 1-click download and configuration with pause, resume, and cancel controls.
- **TransNet V2**: Automatically copies the model if DeadFrameTools is installed, or downloads it directly from GitHub release with pause, resume, and cancel support.
- **Native Project Files (`.bcp`)**: Save sessions, work areas, and cut selections to lightweight project files.

---

## 📥 Installation

1. Go to the **[Releases](https://github.com/zexexwashere/BeforeCuts/releases)** page.
2. Download **`BeforeCuts_Setup.exe`**.
3. Run the installer:
   - Installs **Before Cuts** to your system.
   - Automatically registers `.bcp` (Before Cuts Project) and `.cuts` file associations.
   - Installs the **After Effects extension** into your Adobe extensions folder.
   - Sets up **FFmpeg** in `C:\ffmpeg` if not already installed.
4. Launch **Before Cuts**!

---

## 🚀 Quick Workflow

```
[Import Video] ➔ [Set In/Out (Optional)] ➔ [AI Auto Cut] ➔ [Review & Select Clips] ➔ [Export Scenepack / .cuts]
```

1. **Import**: Drag and drop your video file into the window (or press `Ctrl+O`).
2. **Set Range**: (Optional) Press `I` to set In point, `O` to set Out point.
3. **Detect**: Click **AI Auto Cut** to detect scenes automatically.
4. **Review**: Click any thumbnail in the right panel to loop-preview that cut. Select the ones you want.
5. **Export**: Press `Ctrl+E` to export as a merged scenepack, split clips, or `.cuts` for After Effects.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| **`Space`** | Play / Pause playback |
| **`Left` / `Right`** | Step 1 frame backward / forward |
| **`Shift` + `Left` / `Right`** | Step 1 second backward / forward |
| **`Ctrl` + `Left` / `Right`** | Step 5 seconds backward / forward |
| **`I`** or **`B`** | Set In point at playhead |
| **`O`** or **`N`** | Set Out point at playhead |
| **`Shift`** *(while dragging range)* | Snap In/Out marker to playhead, start, or end |
| **`F11`** or **`F`** | Toggle Fullscreen mode |
| **`M`** | Toggle Audio Mute |
| **`V`** or **`Ctrl` + `B`** | Toggle Videos / Media Bin |
| **`Ctrl` + `N`** | New Project |
| **`Ctrl` + `O`** | Open Project (`.bcp`) |
| **`Ctrl` + `S`** | Save Project (`.bcp`) |
| **`Ctrl` + `Shift` + `S`** | Save Project As... |
| **`Ctrl` + `W`** | Close Current Project |
| **`Ctrl` + `E`** | Open Export Dialog |
| **`Ctrl` + `Z`** | Undo cut selection / edit |
| **`Ctrl` + `Y`** / **`Ctrl` + `Shift` + `Z`** | Redo cut selection / edit |
| **`Esc`** | Exit Isolated Cut Preview / Close Popups & Modals |

---

## 💻 System Requirements

- **OS**: Windows 10 or Windows 11 (64-bit)
- **GPU**: DirectX 12 compatible GPU (NVIDIA GeForce, AMD Radeon, Intel Arc / Iris Xe) for DirectML AI acceleration. CPU fallback is available.
- **Storage**: ~300 MB free space.
- **Video Engine**: FFmpeg installed in `C:\ffmpeg` (automatically configured via 1-click installer).

---

## ⚖️ License & Legal Notice

**Before Cuts** is developed by **Zexex**. All rights reserved (Proprietary / Closed Source).

*Adobe and Adobe After Effects are registered trademarks of Adobe Inc. Before Cuts is an independent tool and is not affiliated with, endorsed by, or sponsored by Adobe Inc.*
