# AR Street Sign — WebXR (Minimal)

Single‑page, WebXR‑only AR experience using `<model-viewer>`. No A‑Frame, AR.js, or MindAR.

## Structure

```
AR-Street-Sign-WebXR-for-Lagree/
├── index.html                 # Model preview + AR (one page)
├── vercel.json                # GLB headers + rewrite
├── AR-Sandwhich-board-upright.glb
└── AR-Sandwhich-board-upright.usdc
```

## Steps

1) Copy your GLB export into the project root as `AR-Sandwhich-board-upright.glb`.
   - Source: `/Users/joshjacobson/Documents/GitHub/AR-Street-Sign-Demo-for-Lagree/AR-Sandwhich-board-upright.glb`
2) (Optional) Export USD/USDZ and place next to the GLB as `AR-Sandwhich-board-upright.usdc` for iOS Quick Look.
3) Open `index.html` locally, or deploy to Vercel.

## Notes

- This is intentionally minimal to emulate the stability of your `lagree-ar` sample.
- Animations: the GLB’s single clip is auto‑played. If clip name changes, update `animation-name`.
- Vercel config sets MIME for `.glb` under `/assets/`.
