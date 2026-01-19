# videomaking

This repository is used to plan, script, and produce YouTube videos.

## Recommended Tooling
This repo favors an **Open Source** and **Scriptable** workflow:
- **Video Assembly:** [Kdenlive](https://kdenlive.org/) (GUI) + [MLT Framework](https://www.mltframework.org/) (CLI).
    - *Why:* Kdenlive provides the timeline; MLT allows headless rendering and XML manipulation.
- **Processing:** [FFmpeg](https://ffmpeg.org/) (CLI).
    - *Why:* The gold standard for transcoding, audio extraction, and batch processing.
- **Analysis/Charts:** Python ([Matplotlib](https://matplotlib.org/), [Pandas](https://pandas.pydata.org/)).
    - *Why:* Scripts generate the charts/data visualizations as PNG/SVG, which are then dropped into the editor.
- **Recording:** [OBS Studio](https://obsproject.com/).

## Workflow
1.  **Planning:** Write scripts and data analysis in `projects/<video-name>/`.
2.  **Asset Generation:** Run Python scripts to generate charts into `assets/`.
3.  **Editing:** Use Kdenlive to arrange footage and assets.
4.  **Automation:** Use FFmpeg for preprocessing raw footage (e.g., normalized audio, proxies).
5.  **Render:** Export final video to `exports/`.

## What lives here
- Video ideas, outlines, and scripts
- Project notes (titles, descriptions, tags)
- Assets that are safe to version-control (thumbnails source files, small graphics, templates)
- Links and references to raw footage stored elsewhere

## What should NOT be committed
Raw footage and large renders are typically too big for git. Prefer external storage or Git LFS.

## Suggested layout
- `projects/` — one folder per video (script, notes, metadata)
- `assets/` — reusable graphics, templates, music (license permitting)
- `thumbnails/` — thumbnail source files
- `exports/` — final rendered outputs (ignored by git)
- `raw/` — raw recordings/footage (ignored by git)

## Notes
- If you need to version large binaries, consider Git LFS.
