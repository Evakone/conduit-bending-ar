# AR Street Sign — WebXR (Minimal)

Single‑page, WebXR‑only AR experience using `<model-viewer>`. No A‑Frame, AR.js, or MindAR.

## Structure

```
AR-Street-Sign-WebXR-for-Lagree/
├── index.html                 # Model preview + AR (one page)
├── vercel.json                # GLB headers + rewrite
└── assets/
    └── models/
        └── AR-Sandwich-board-v2.optim.glb  # PLACE HERE (copy from other project)
        └── AR-Sandwich-board-v2.usdz       # Optional for iOS Quick Look
```

## Steps

1) Copy your optimized GLB (~0.8MB) into `assets/models/` as `AR-Sandwich-board-v2.optim.glb`.
   - Source: `/Users/joshjacobson/Documents/GitHub/AR-Street-Sign-Demo-for-Lagree/AR-Sandwich-board-v2.optim.glb`
2) (Optional) Export USDZ and place next to GLB as `AR-Sandwich-board-v2.usdz` for iOS Quick Look.
3) Open `index.html` locally, or deploy to Vercel.

## Notes

- This is intentionally minimal to emulate the stability of your `lagree-ar` sample.
- Animations: the GLB’s single clip is auto‑played. If clip name changes, update `animation-name`.
- Vercel config sets MIME for `.glb` under `/assets/`.

