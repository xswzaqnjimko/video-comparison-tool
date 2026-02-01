# Video Comparison Tool

A lightweight, browser-based tool for synchronized multi-video comparison. Helps presentations, A/B testing, side-by-side analysis, or your choice.
Made for research use; encouraged to put it onto GitHub.

## Features

V1.4 2026/02/01

- **Synchronized Playback** - All videos play, pause, and seek together
- **Drag & Rearrange** - Reorder video panels by dragging
- **Overlay Mode** - Stack videos with adjustable transparency for direct comparison
- **Zoom Lens** - Hold Shift + hover to magnify video details (2.5x zoom, synchronized across panels)
- **Auto-Replay** - Loop videos continuously (toggleable)
- **Flexible Layout** - Support for 1-10 videos with responsive grid
- **Fullscreen viewing** - Enlarge to better see
- **Zero Dependencies** - Single HTML file, works offline

## Quick Start

1. Download `video_comparison.html`
2. Open in any modern browser
3. Upload your videos (click or drag)
4. Compare!

## Usage

### Controls

| Button | Function |
|--------|----------|
| Videos: [1-10] | Set number of comparison panels (can type directly); auto fits bulk upload video amount |
| 🗑️ Clear All | Remove all uploaded videos |
| ▶️ Play/Pause | Start/stop all videos simultaneously |
| Reset | Return all videos to beginning |
| 🔁 Loop | Toggle auto-replay on/off |
| Speed | Playback speed (0.25x - 2x) |
| 🏷️ Tags | Toggle video name labels on/off |
| Shift | Hold Shift to view zoom lens (2.5x) |
| 🔲 Overlay | Enable overlay mode for stacking videos |
| ⚡ Flicker | In overlay mode, auto-switch between top/bottom video |
| 🔲 Clear | In overlay mode, remove all overlays |

### Bulk Upload

Drag multiple video files at once onto the video grid area. Videos will be:
- Automatically sorted by filename
- Panel count auto-expands to fit (up to 10)
- You can still rearrange after upload

### Rearranging Videos

Simply drag any video panel and drop it onto another to swap positions.

### Zoom Lens

Hold **Shift** while hovering over any video panel to activate the zoom lens:
- Circular magnifying glass appears at cursor position
- 2.5x magnification of video content
- Works in both normal and overlay modes
- Synchronized position across all panels for easy comparison

### Overlay Comparison

1. Click "Overlay" button to enable overlay mode
2. Drag one video onto another
3. Adjust opacity with the slider
4. Click "Clear" to reset
5. Click on panel to switch/compare top/bottom video. Or use Flicker mode for auto switching
6. *Still working on UI etc.

## TODO...

1. [ ] Press Space to pause, ⬅️/➡️ to adjust, etc.
2. [ ] Frame-by-frame drag-to-play
3. [ ] Adjustable zoom lens scale (e.g. 2x-4x)
4. [ ] Hover to show data detail...
5. [ ] etc.

## License

MIT License - see [LICENSE](LICENSE)

