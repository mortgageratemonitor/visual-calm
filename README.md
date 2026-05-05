# Visual Calm

A browser-based generative visual experience designed for relaxation and focus. Four immersive modes run entirely in your browser with no backend, no login, and no time limit — safe to leave running for hours.

---

## Modes

### Warp
You are traveling through deep space at warp speed. Colorful tunnel rings surround you while thousands of stars stretch into streaking lines of light as you accelerate. Mouse movement subtly tilts your trajectory.

A **Pulse** toggle sits in the bottom-right corner. When enabled, the ship surges every ~9 seconds — the tunnel compresses, stars blur outward dramatically, then everything settles back to cruising speed. Toggle it off for a dense, steady starfield and a calmer experience.

### Black Hole
An orbital view of a supermassive black hole. A bright photon ring (Einstein ring) wraps tightly around the event horizon, with a secondary arc tilted slightly off-axis. The accretion disk rotates with visible density clumps, color shifting from near-white at the inner edge through orange and deep red to a purple outer fringe.

Background stars bend and warp toward the singularity due to gravitational lensing. The camera slowly breathes — drifting closer then pulling back on a 28-second cycle — with fog deepening as you approach. Mouse nudges your viewing angle.

### Kaleidoscope
A geometric mandala that continuously evolves. The source pattern is built from rotating polygon rings (triangle, square, hexagon, octagon, dodecagon), four rings of orbiting dot clusters, radiating laser lines from the center, and a pulsing bloom — all reflected across 16 mirrored segments. Color cycles slowly through the full spectrum.

### Forest Stream
You drift slowly above a forest stream. A rippling water surface below you animates with layered sine-wave displacement. Caustic light blobs dance on the water, simulating the patterns sunlight makes through moving water. Glowing pollen and spores drift upward through god-ray light shafts that breathe through a dark overhead canopy. Fireflies pulse in and out. Mouse gently sways your view side to side.

---

## Controls

- **Mode buttons** — bottom center pill, switches between the four scenes
- **Pulse toggle** — bottom right, Warp mode only
- **Mouse** — subtly influences every scene; UI auto-hides after 3.5 seconds of inactivity and reappears on movement

---

## Technical Notes

- Built with [Three.js](https://threejs.org/) (r128) and vanilla Canvas 2D (Kaleidoscope)
- Single `index.html` — no build step, no dependencies to install
- Frame rate capped at 30fps; full memory cleanup on every scene switch
- Designed to run for 1+ hours without degradation
- Hosted via GitHub Pages (static, always-on, no cold starts)
