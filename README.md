# Shankh AR — WebAR Avatar

**Live demo:** [ar-bye.vercel.app](https://ar-bye.vercel.app)

A browser-based augmented reality experience that brings **Shankh**, a 3D avatar from my AR/VR Indic financial chatbot, into the real world. Point your phone camera at the marker image and the animated avatar appears anchored to it. No app install needed.

![Shankh AR preview](AR.png)

## How it works

- **Image tracking:** [MindAR](https://github.com/hiukim/mind-ar-js) tracks a printed marker, compiled into `targets.mind` from `marker.jpg`.
- **Scene:** [A-Frame](https://aframe.io) handles the AR scene and camera.
- **Avatar:** a Draco-compressed GLB model (`ar.glb`) loaded with Three.js `GLTFLoader` and played with an `AnimationMixer`.

## Try it

1. Open the [live demo](https://ar-bye.vercel.app) on your phone and allow camera access.
2. Tap **Start**.
3. Point the camera at [`marker.jpg`](marker.jpg), shown on another screen or printed.

## Files

| File | Purpose |
|---|---|
| `ar_new.html` | The WebAR page |
| `ar.glb` | Animated 3D avatar (Draco-compressed glTF) |
| `marker.jpg` | Image target to point the camera at |
| `targets.mind` | Compiled MindAR image-target data |
| `AR.png` | Preview image |

## Tech

WebAR · MindAR · A-Frame · Three.js · glTF/GLB · Blender
