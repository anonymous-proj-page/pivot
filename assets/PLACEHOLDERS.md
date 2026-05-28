# Media manifest

Drop the real files at the exact paths below. Each slot in `index.html` already has a commented
`<video>` / `<img>` tag right next to its placeholder — uncomment it and delete the placeholder
`<div>` once the file exists.

Keep everything **local** — do not link to external/hosted media (anonymity requirement).

## Videos (`assets/videos/`)

| File | Section | Suggested aspect | Notes |
|------|---------|------------------|-------|
| `teaser.mp4` | Hero / 4-task flash montage | 16:9 | Short fast-cut montage of all four tasks. Autoplay, muted, loop. |
| `main.mp4` | Overview | 16:9 | Main narrated/overview video. Has playback controls. |
| `laundry_1h.mp4` | Continuous Tasks | 16:9 | Continuous laundry folding, ~1 hour (or sped-up). Autoplay, muted, loop. |
| `ziptie_1h.mp4` | Continuous Tasks | 16:9 | Continuous zip-tie threading, ~1 hour. Autoplay, muted, loop. |
| `sachet_x10.mp4` | Continuous Tasks | 16:9 | 10 consecutive sachet runs. Autoplay, muted, loop. |
| `paperbox_x10.mp4` | Continuous Tasks | 16:9 | 10 consecutive paper-box assemblies. Autoplay, muted, loop. |
| `generalization_colored_ziptie.mp4` | Generalization | 16:9 | Threading colored cable ties (unseen appearance). Autoplay, muted, loop. |

**Format tips:** H.264 MP4 (`yuv420p`) for broad browser support; web-optimize with
`-movflags +faststart`. Keep autoplay-loop clips reasonably small.

## Images (`assets/images/`)

| File | Section | Suggested aspect | Notes |
|------|---------|------------------|-------|
| `fig_iterative.png` | Experiments | wide (~16:6) | Iterative improvement across tasks (per-iteration success/throughput). |
| `fig_comparison.png` | Experiments | wide (~16:6) | Policy-extraction comparison & ablations. |
| `fig_multitask.png` | Experiments | wide (~16:6) | Unified multi-task post-training. |

Adjust each slot's `--ratio` in `index.html` (e.g. `style="--ratio:16/6"`) to match the real
asset's proportions so the layout stays tight.
