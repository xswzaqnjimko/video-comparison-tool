# Contributing to Video Comparison Tool

## Creating Experiment Branches

For experiment-specific versions with custom datasets:

### 1. Create a new branch

```bash
git checkout -b experiment/your-experiment-name
```

### 2. Branch naming convention

- `experiment/ring-temperature` - Ring temperature visualization
- `experiment/fluid-dynamics` - Fluid simulation comparison
- `experiment/motion-tracking` - Motion tracking analysis

### 3. Structure for experiment branches

```
video-comparison-tool/
├── index.html          # Modified with your data integration
├── data/
│   ├── dataset.json    # Your experiment data
│   └── metadata.json   # Data descriptions
└── README.md           # Experiment-specific documentation
```

### 4. Data Integration

Modify the `generateMockData` function to load your actual data:

```javascript
// Example: Loading from embedded JSON
const experimentData = {
    // Your data here
};

const getExperimentData = (videoLabel, time, position) => {
    // Your lookup logic
    return {
        temperature: ...,
        pressure: ...,
        // etc.
    };
};
```

### 5. Keeping private data private

If your dataset is sensitive:

- **Option A**: Keep experiment branch in a separate private repository
- **Option B**: Use `.gitignore` to exclude data files, load them separately
- **Option C**: Keep branch local, never push to public repo

Example `.gitignore` for experiment branches:
```
data/*.csv
data/*.json
!data/sample.json
```

## General Contributions

### Bug Fixes & Features

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Make your changes
4. Test in multiple browsers
5. Submit a pull request

### Code Style

- Keep it simple - single HTML file preferred for main tool
- Comment complex logic
- Test with various video formats and counts

## Questions?

Open an issue for discussion.
