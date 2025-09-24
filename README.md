# Conduit Bending in AR — WebXR Demo

Single‑page, WebXR‑only AR experience using `<model-viewer>` for electrical conduit bending education. No A‑Frame, AR.js, or MindAR.

## Structure

```
Conduit-Bending-AR/
├── index.html                 # Model preview + AR (one page)
├── vercel.json                # Asset headers + rewrite
├── Conduit bending in AR.glb
├── Conduit bending in AR.usdz
└── Conduit bending in AR.usdc  # Source USD (packaged inside USDZ)
```

## Features

- **WebXR AR Support**: Works on both Android (WebXR) and iOS (Quick Look)
- **Camera Access**: Prompts for camera permission before AR activation
- **Interactive Controls**: Scale adjustment and touch controls for model manipulation
- **Sask Polytech Branding**: Educational institution branding and citation

## Steps

1) Ensure your GLB and USDC files are in the project root:
   - `Conduit bending in AR.glb` (for WebXR/Android)
   - `Conduit bending in AR.usdc` (source USD file)
2) Create a USDZ bundle for iOS Quick Look:
   ```sh
   usdzip "Conduit bending in AR.usdz" "Conduit bending in AR.usdc"
   ```
   - Requires Xcode Command Line Tools (for `usdzip`).
3) Open `index.html` locally, or deploy to Vercel.

## Notes

- **Educational Focus**: Designed for electrical conduit bending training at Sask Polytech
- **Cross-Platform**: Supports both Android (WebXR) and iOS (Quick Look) AR
- **Minimal Design**: Clean, focused interface for educational use
- **Camera Integration**: Proper camera permission handling for AR functionality
