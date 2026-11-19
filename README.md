# KUN STREET RACING

Mobile-first 3D street-driving prototype built with Three.js.

## Run
Serve this folder from a local or static web server (ES modules and model loading require HTTP/HTTPS). Open `index.html` through that server.

## Controls
- W / Up: throttle
- S / Down / Space: brake
- A / Left and D / Right: steering
- C or CAMERA: switch camera
- RESET: return to start

## Asset status
The source project expects these files:
- `assets/car/source/Silvia S14 URAS Slime.glb`
- `assets/city/source/city-cpm.fbx`
- City texture files under `assets/city/textures/`

Large 3D assets are not included in this initial source commit. Add them with Git LFS or a suitable asset host; do not commit files larger than GitHub's 100 MB per-file limit. If the car model is absent, the page uses a simple placeholder car. The city currently falls back to a flat test surface until its FBX and textures are added.

## Notes
This is an early driving prototype, not a complete CarX Street-scale game.