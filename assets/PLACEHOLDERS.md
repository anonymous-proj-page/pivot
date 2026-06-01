# Media manifest

Drop the real files at the exact paths below. Each slot in `index.html` already has a commented
`<video>` / `<img>` tag right next to its placeholder — uncomment it and delete the placeholder
`<div>` once the file exists.

Keep everything **local** — do not link to external/hosted media (anonymity requirement).

## Videos (`assets/videos/`)

| File | Section | Suggested aspect | Notes |
|------|---------|------------------|-------|
| `laundry_1h.mp4` | Continuous Tasks (hook) | 16:9 | **Highlighted** one-hour continuous T-shirt folding. Autoplay, muted, loop. |
| `laundry_4garments.mp4` | Continuous Tasks (grid) | 16:9 | Continuous folding across four different garments. Autoplay, muted, loop. |
| `ziptie_1h.mp4` | Continuous Tasks (grid) | 16:9 | Continuous zip-tie threading, ~1 hour. Autoplay, muted, loop. |
| `sachet_4pairs.mp4` | Continuous Tasks (grid) | 16:9 | Success across four different sachet pairs. Autoplay, muted, loop. |
| `paperbox.mp4` | Continuous Tasks (grid) | 16:9 | Already present. Autonomous box assembly, shown at 20×. Autoplay, muted, loop. |
| `generalization_tshirt.mp4` | Generalization | 16:9 | Folding unseen T-shirts. Autoplay, muted, loop. |
| `generalization_ziptie.mp4` | Generalization | 16:9 | Threading colored cable ties (unseen appearance). Autoplay, muted, loop. |
| `robustness_disturbance.mp4` | Robustness | 16:9 | Folding under physical human disturbance. Autoplay, muted, loop. |
| `robustness_refold.mp4` | Robustness | 16:9 | Self-correction: re-folds after a poor result. Autoplay, muted, loop. |
| `robustness_recovery.mp4` | Robustness | 16:9 | Recovery from a small execution slip mid-fold. Autoplay, muted, loop. |
| `robustness_lighting.mp4` | Robustness | 16:9 | Folding under varied lighting. Autoplay, muted, loop. |

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
