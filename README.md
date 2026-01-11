# Video Comparison Tool

A lightweight, browser-based tool for synchronized multi-video comparison. Perfect for research presentations, A/B testing, and side-by-side analysis.
Made for research use; encouraged to put it onto GitHub.

## Features

- **Synchronized Playback** - All videos play, pause, and seek together
- **Drag & Rearrange** - Reorder video panels by dragging
- **Overlay Mode** - Stack videos with adjustable transparency for direct comparison
- **Auto-Replay** - Loop videos continuously (toggleable)
- **Hover Data Labels** - View data at cursor position across all videos
- **Flexible Layout** - Support for 1-10 videos with responsive grid
- **Drag-to-Upload** - Drop video files directly onto panels
- **Zero Dependencies** - Single HTML file, works offline

## Quick Start

1. Download `index.html`
2. Open in any modern browser
3. Upload your videos (click or drag)
4. Compare!

## Usage

### Controls

| Button | Function |
|--------|----------|
| Videos: [1-10] | Set number of comparison panels (type directly) |
| 🗑️ Clear All | Remove all uploaded videos |
| ▶️ Play/Pause | Start/stop all videos simultaneously |
| 🔄 Reset | Return all videos to beginning |
| 🔁 Loop | Toggle auto-replay on/off |
| Speed | Playback speed (0.25x - 2x) |
| 📑 Overlay | Enable overlay mode for stacking videos |
| 🔲 Clear | Remove all overlays |

### Bulk Upload

Drag multiple video files at once onto the video grid area. Videos will be:
- Automatically sorted by filename
- Panel count auto-expands to fit (up to 10)
- You can still rearrange after upload

### Video Count

Adjust (input or click) the "Videos" number input (1-10) to add or remove comparison panels.

### Rearranging Videos

Simply drag any video panel and drop it onto another to swap positions.

### Overlay Comparison

1. Click "Overlay" button to enable overlay mode
2. Drag one video onto another
3. Adjust opacity with the slider
4. Click "Clear" to reset
5. *Still working on its UI etc.

### Hover Data

Hover over any video to see synchronized data labels for all videos at that position.
*Still working. Currently showing mock data.

## Hosting

### GitHub Pages (Recommended)

1. Fork this repository
2. Go to Settings → Pages
3. Select "Deploy from a branch" → `main`
4. Your tool will be live at `https://yourusername.github.io/video-comparison-tool/`

### Other Options

- **Netlify**: Drag the folder to [netlify.com/drop](https://app.netlify.com/drop)
- **Vercel**: Import the repository
- **Local**: Just open `index.html` in a browser

## Customization

### For Specific Experiments

Create a branch for your experiment with custom data integration:

```bash
git checkout -b experiment/your-experiment-name
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on creating experiment branches.

### Modifying Data Labels

Edit the `generateMockData` function in `index.html` to integrate your own dataset:

```javascript
const generateMockData = (videoType, frameTime, ringPosition) => {
    // Replace with your data lookup logic
    return {
        index: yourData.getValue(frameTime, ringPosition),
        time: frameTime.toFixed(2) + 's',
        position: (ringPosition * 360 / 100).toFixed(1) + '°'
    };
};
```

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

## License

MIT License - see [LICENSE](LICENSE)

## Contributing

Contributions welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.
