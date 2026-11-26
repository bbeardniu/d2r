# D2R Battle Orders Timer

A self-contained GitHub Pages timer for Diablo II: Resurrected.

## Publish on GitHub Pages
1. Create a GitHub repository (for example, `d2r-bo-timer`).
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Open the Pages URL GitHub provides.

## Duration calculation
The timer uses:

`30 + 10 × (Battle Orders level − 1) + 5 × (Shout hard points + Battle Command hard points)`

Select the effective Battle Orders level, including +skills from gear. The synergy fields are hard points only. The duration formula and per-level progression are based on current D2R skill data.

## Audio trigger limitations
The optional audio trigger uses the browser's screen/tab-sharing permission and audio amplitude spikes. When prompted, share the Diablo II game tab/window and enable audio sharing. It does **not** identify the Battle Orders sound specifically; other loud sounds may trigger it, and quiet/overlapping casts may be missed. The manual button is the dependable option. Browser support and system audio capture vary; desktop Chrome/Edge are the best candidates.

## Notes
- No external libraries, network requests, or build step.
- The timer continues while this page remains open.
- The sound chime is generated locally with Web Audio.
- The emblem is original inline artwork rather than an extracted game asset.
