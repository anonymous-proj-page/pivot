# Media manifest

Drop the real files at the exact paths below. Each slot in `index.html` already has a commented
`<video>` / `<img>` tag right next to its placeholder — uncomment it and delete the placeholder
`<div>` once the file exists.

Keep everything **local** — do not link to external/hosted media (anonymity requirement).

## Videos (`assets/videos/`)

| File | Section | Suggested aspect | Notes |
|------|---------|------------------|-------|
| `main.mp4` | Top promo | 16:9 | Main promo video at the top of the page. Has playback controls. |
| `laundry_1h.mp4` | Continuous Tasks | 16:9 | Continuous laundry folding, ~1 hour. Autoplay, muted, loop. |
| `ziptie_1h.mp4` | Continuous Tasks | 16:9 | Continuous zip-tie threading, ~1 hour. Autoplay, muted, loop. |
| `sachet_x10.mp4` | Continuous Tasks | 16:9 | 10 consecutive sachet runs. Autoplay, muted, loop. |
| `paperbox_x10.mp4` | Continuous Tasks | 16:9 | 10 consecutive paper-box assemblies. Autoplay, muted, loop. |
| `generalization_tshirt.mp4` | Generalization | 16:9 | Folding unseen T-shirts. Autoplay, muted, loop. |
| `generalization_ziptie.mp4` | Generalization | 16:9 | Threading colored cable ties (unseen appearance). Autoplay, muted, loop. |
| `robustness_recovery.mp4` | Robustness | 16:9 | Recovery from disturbances on Laundry + Zip-Tie (combined). Autoplay, muted, loop. |
| `robustness_lighting.mp4` | Robustness | 16:9 | Lighting variations on Laundry + Zip-Tie (combined). Autoplay, muted, loop. |

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
