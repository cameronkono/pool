# 8ENERATOR

One file: `index.html`.

Open it in a browser (Chrome / Arc / Safari). The first load needs internet for Three.js and Tailwind from a CDN. After that, the tool itself is just this file — nothing is uploaded.

Drop a `.glb`, `.gltf`, `.obj`, or `.fbx` to view a model, or a still / video (`.png`, `.jpg`, `.webp`, `.mp4`, `.webm`) to run the 2D effects on that instead. Orbit, zoom, and pan in 3D, or set Orbit / Height / Distance in the camera panel. Hide the panel when you want the full viewport.

## Controls

Source, material, lighting, environment, background, and camera live in the right-hand panel. Switch Source to **Image / Video** to grade a still or a muted looping video — Pause holds a video on the current frame. Blob tracker, gradient map, blur, and film grain sit below camera — off by default, so the viewer stays as fast as a plain render until you turn one on. Those effects are processed only on the contained image or video pixels, not the letterbox. Order is grade → blur → grain, then blob boxes and labels, so tracker colors stay as picked; brightness / contrast still apply before the grade. **Save PNG** writes a still at 1–4× the viewport, including effects. Set Background to None for a transparent image. **Save recipe** downloads the current panel look and camera (orbit, perspective / ortho, FOV) as JSON; drop that file later (or use Load recipe) to restore it without the model or clip.
