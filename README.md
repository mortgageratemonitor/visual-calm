# Cosmic Calm

A browser-based generative visual experience designed for relaxation and focus. Four immersive modes run entirely in your browser with no backend, no login, and no time limit — safe to leave running for hours.

---

## Modes

### Warp
You are traveling through deep space at warp speed. Colorful tunnel rings surround you while thousands of stars stretch into streaking lines of light as you accelerate. Stars close to the tunnel axis pick up color from the rings; stars further out fade toward white. A deep blue-purple fog gives the tunnel real depth. Mouse movement subtly tilts your trajectory.

A **Pulse** toggle sits in the bottom-right corner. When enabled, the ship surges every ~9 seconds — the tunnel compresses, stars blur outward dramatically, then everything settles back to cruising speed. Toggle it off for a denser starfield (16,000 stars vs 7,000) and a calmer, steady experience.

### Black Hole
An orbital view of a supermassive black hole. A bright photon ring (Einstein ring) wraps tightly around the event horizon, with a secondary arc tilted slightly off-axis — both pulse gently in brightness. The accretion disk rotates with visible density clumps across 20,000 particles, color shifting from near-white at the inner edge through orange and deep red to a purple outer fringe.

Background stars bend and warp toward the singularity, simulating gravitational lensing. The camera slowly breathes — drifting closer then pulling back on a 28-second cycle — with fog deepening as you approach. Mouse nudges your viewing angle.

### Kaleidoscope
A fully interactive geometric mandala. The source pattern layers rotating polygon rings (triangle, square, hexagon, octagon, dodecagon), four rings of orbiting dot clusters, spirograph-style Lissajous curves with irrational frequency ratios that never quite repeat, and radiating laser lines from a pulsing center bloom.

**Mouse controls:**
- **Move left/right** — spins the entire kaleidoscope. Fast movements carry momentum that decays naturally, like spinning a physical object
- **Move up/down** — zooms the source pattern in and out
- **Distance from center** — the further your cursor is from the center of the screen, the more mirror segments appear (8 → 32), multiplying the reflections in real time

**Color mode** cycles automatically every 60 seconds: warm (oranges/reds) → full spectrum → cool (blues/cyans/purples) → monochrome (silver/white) → back to warm.

### Forest Stream
You drift slowly above a forest stream. A subdivided water mesh animates with layered sine-wave ripples and a pulsing shimmer layer on top. Caustic light blobs dance on the water surface, simulating the patterns sunlight makes through moving water. Glowing pollen and spores drift lazily upward through god-ray light shafts that breathe through a dark overhead canopy of swaying leaves. Fireflies pulse in and out. Mouse gently sways your view side to side.

---

## Controls

| Input | Effect |
|-------|--------|
| **Mode buttons** | Bottom center pill — switches between the four scenes |
| **Pulse toggle** | Bottom right — Warp mode only, enables/disables speed surges |
| **Mouse move** | Subtly influences every scene; see Kaleidoscope for full interactivity |

UI auto-hides after 3.5 seconds of inactivity and reappears on any mouse movement.

---

## Technical Notes

- Built with [Three.js](https://threejs.org/) (r128) and vanilla Canvas 2D (Kaleidoscope)
- Single `index.html` — no build step, no dependencies to install
- Frame rate capped at 30fps; full memory cleanup on every scene switch
- Designed to run for 1+ hours without degradation
- Hosted via GitHub Pages (static, always-on, no cold starts)
