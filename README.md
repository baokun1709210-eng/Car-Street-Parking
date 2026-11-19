# KUN STREET RACING

A mobile-first 3D street-driving prototype built with Three.js.

## Current build
- Three.js renderer with mobile touch controls and keyboard controls
- FBX city-map loader with local texture lookup
- Silvia S14 URAS Slime GLB loader
- Fallback practice ground and placeholder car if an asset is missing
- GitHub Pages deployment workflow at `.github/workflows/pages.yml`

## Required asset layout
Upload the extracted files from the two supplied archives into these exact paths:

```
assets/
  city/
    source/
      city-cpm.fbx
    textures/
      (all PNG/JPG files from the city archive's textures folder)
  car/
    source/
      Silvia S14 URAS Slime.glb
    textures/
      (all texture files from the car archive's textures folder)
```

The FBX is approximately 91.8 MB and the GLB approximately 49.7 MB. Both are below GitHub's 100 MB per-file hard limit, but the city ZIP archive itself is larger than 100 MB. Upload extracted files, not the ZIP archive. Large files can be uploaded through GitHub's web interface or Git LFS; this repository currently contains the loader code, not the binary 3D assets.

## Run
Open the repository's GitHub Pages URL after Pages is configured to deploy from GitHub Actions, or serve the repository root over HTTP/HTTPS. ES modules and model loaders do not work reliably from a `file://` URL.

## Controls
- W / Up: throttle
- S / Down / Space: brake
- A / Left and D / Right: steering
- C or CAMERA: switch camera
- RESET: return to the starting position

## Scope
This is an early free-roam driving prototype, not a complete CarX Street-scale game.