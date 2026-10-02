# Face Swap

Standalone browser page that copies a face onto a photo or video. Detection and warping run locally. Nothing is uploaded.

Open `index.html` in Chrome or Edge. The first load downloads the MediaPipe face model (~3 MB).

## Use

1. Wait for **Model ready**.
2. Drop the face to copy, then the photo or video to put it on. Click a face chip if more than one is found.
3. Or switch to **Swap two faces in one photo**.
4. **Swap faces** for a still. **Render video** for a clip (WebM, audio kept in Chrome).

This is a landmark warp, not a neural deepfake. Front-facing faces of similar size and light work best.

If the model will not load from a double-clicked file, serve the folder and open the local URL:

```bash
python -m http.server
```
