# videomaking

This repository is used to plan, script, and produce YouTube videos.

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
