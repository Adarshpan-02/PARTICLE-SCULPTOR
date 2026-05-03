# Particle Sculptor

Upload a photo. Watch it become a 3D particle cloud you can actually explore.

Live Site (particle-sculptor.netlify.app/)

## What it does

Particle Sculptor takes any image and rebuilds it as a three-dimensional point cloud. Every pixel becomes a particle positioned in space — brighter areas push toward you, darker areas recede — so the result has real depth, not just the illusion of it.

You can rotate the model freely, zoom in until individual particles fill the screen, or pan around to see it from any angle. It feels different from just looking at a photo. That's the point.

## Features

**Background removal** — Before building the model, you can strip out dark or light backgrounds so you're sculpting the subject, not a rectangle.

**Real image colors** — Particles carry the actual RGB values from your photo. You can also switch to grayscale or inverted grayscale if that's what you're after.

**Live controls** — Density, depth scale, and background threshold all update the model in real time as you drag the sliders. No regenerate button required.

**3D export** — Download the result as an OBJ or PLY file. Open it in Blender, MeshLab, or anything else that reads point cloud data.

**Screenshot** — Save the current viewport exactly as it looks.

**Runs in the browser** — One HTML file, no server, no account, nothing uploaded anywhere.

## How to use it

1. Open the file in any modern browser
2. Drop in an image (JPG, PNG, WEBP)
3. Adjust the controls on the left — the model updates live
4. Rotate with left-click drag, zoom with scroll, pan with right-click drag
5. Export when you're happy with it

## Controls

| Control | What it does |
|---|---|
| Density | Number of particles in the model |
| Depth Scale | How much the brightness difference translates into Z-depth |
| Particle Size | Size of each point (updates instantly) |
| BG Threshold | How aggressively the background gets removed |
| Background Remove | Remove dark bg, light bg, or keep everything |
| Color Mode | Real colors, grayscale, or inverted |
| Animation | Breathe, auto-rotate, wave, or static |

## Tips

- Photos with a clear subject against a plain background work best
- If the model looks flat, try increasing the Depth Scale
- If background particles are showing up, increase the BG Threshold
- Density above 80k starts to get slow on lower-end machines — worth knowing before you push it to 150k

## Export formats

**OBJ** — Standard format, opens in basically everything  
**PLY** — Point cloud format with per-vertex color data, good for MeshLab and 3D printing workflows

---

Single file. No dependencies to install. Just open it.
