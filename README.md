# Video Comparison Tool

A lightweight, browser-based tool for synchronized multi-video comparison.
Useful for presentations, A/B testing, side-by-side analysis, and general visual comparison.

Use here: [**Video Comparison Tool**](https://xswzaqnjimko.github.io/video-comparison-tool/)

## Features

Version 1.5 (2026-04-02)

- **Synchronized playback** — all videos play, pause, and seek together
- **Drag and rearrange** — reorder video panels by dragging
- **Overlay mode** — stack videos with adjustable transparency for direct comparison
- **Zoom lens** — hold Shift and hover to magnify details (2.5× zoom, synchronized across panels)
- **Auto-replay** — loop videos continuously
- **Flexible layout** — supports 1–10 videos with a responsive grid
- **Fullscreen viewing** — enlarge panels for easier inspection
- **Zero dependencies for users** — just open the page and load videos
- **Online use** - Deployed on GitHub Pages

## Use online with GitHub Pages

https://xswzaqnjimko.github.io/video-comparison-tool/


## Use locally

1. Download `index.html`
2. Open it in any modern browser
3. Add videos by clicking or dragging files in
4. Compare
5. Adjust for more features as your need

## Controls

| Button | Function |
|--------|----------|
| Videos: [1-10] | Set number of comparison panels (can type directly); auto-fits bulk upload amount |
| 🗑️ Clear All | Remove all uploaded videos |
| ▶️ Play/Pause | Start or stop all videos simultaneously |
| Reset | Return all videos to the beginning |
| 🔁 Loop | Toggle auto-replay on or off |
| Speed | Playback speed (0.25×–2×) |
| 🏷️ Tags | Toggle video name labels on or off |
| Shift | Hold Shift to show the zoom lens |
| 🔲 Overlay | Enable overlay mode for stacking videos |
| ⚡ Flicker | In overlay mode, auto-switch between top and bottom video |
| 🔲 Clear | In overlay mode, remove all overlays |

## Bulk upload

Drag multiple video files onto the video grid area. Videos will be:

- automatically sorted by filename
- fit into the panel count automatically (up to 10)
- still draggable afterward for manual rearrangement

## Rearranging videos

Drag any video panel and drop it onto another to swap positions.

## Zoom lens

Hold **Shift** while hovering over a video panel to activate the zoom lens:

- circular magnifying glass appears at the cursor position
- 2.5× magnification of video content
- works in both normal and overlay modes
- synchronized position across all panels for easier comparison

## Overlay comparison

1. Click **Overlay** to enable overlay mode
2. Drag one video onto another
3. Adjust opacity with the slider
4. Click **Clear** to reset overlays
5. Click on a panel to switch between top and bottom video, or use **Flicker** mode for auto-switching

## Possible future improvements

- keyboard shortcuts (Space to pause, arrow keys to seek, etc.)
- frame-by-frame or drag-to-scrub controls
- adjustable zoom lens scale
- richer metadata display on hover

## License

MIT License — see [LICENSE](LICENSE)
