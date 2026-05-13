# Cosmic Calm

A browser-based generative visual experience designed for relaxation and focus. Six immersive modes run entirely in your browser with no backend, no login, and no time limit — safe to leave running for hours. Works on desktop and mobile.

---

## Modes

### Warp
You are traveling through deep space at warp speed. Colorful tunnel rings surround you while thousands of stars stretch into streaking lines of light as you accelerate. Stars close to the tunnel axis pick up color from the rings; stars further out fade toward white. A deep blue-purple fog gives the tunnel real depth. Mouse or finger movement subtly tilts your trajectory.

A **Pulse** toggle sits in the bottom-right corner. When enabled, the ship surges every ~9 seconds — the tunnel compresses, stars blur outward dramatically, then everything settles back to cruising speed. Toggle it off for a denser starfield (16,000 stars vs 7,000) and a calmer, steady experience.

### Forest Stream
You drift slowly above a forest stream at golden hour. The scene is built from several layered systems that combine to create a realistic forest environment.

**Water** — a subdivided mesh ripples with layered sine-wave displacement. A reflection layer sits just above it, pulsing in sync with the overhead light shafts to simulate canopy light bouncing off the stream. A shimmer glint layer adds surface sparkle. Expanding ripple rings spawn randomly across the water — like raindrops or fish breaking the surface — growing outward and fading over 2–4 seconds.

**Forest** — 28 three-dimensional trees line the stream, each with a tapered cylinder trunk and 2–3 overlapping foliage sphere clusters. Trees have genuine depth as you pass between them.

**Atmosphere** — two layers of ground mist hug the water surface at different heights, both breathing independently. A green-teal color grading plane follows the camera, tinting the whole scene with a humid forest atmosphere. Caustic light blobs dance across the water surface. God-ray light shafts pulse down through a canopy of 36 swaying leaf planes overhead.

**Particles** — fine dust drifts through the air, glowing pollen and spores float lazily upward, and fireflies pulse in and out near the waterline. Mouse or finger movement gently sways your view side to side.

### Deep Ocean
You drift through a bioluminescent deep sea environment. Blue-green light shafts pierce down from the surface above, casting caustic light patterns across the water below. 1,800 bioluminescent particles pulse in blue, cyan, and teal, drifting slowly through the dark water. 600 bubbles rise steadily upward. 14 jellyfish — built from glowing torus bells and trailing tentacle line segments — pulse and drift in gentle arcs. Mouse or finger movement shifts your view through the water column.

### Sacred Geometry
A meditative 3D geometry experience. Five nested Platonic solids — icosahedron, dodecahedron, octahedron, tetrahedron, and a second icosahedron — rotate on independent axes at different speeds, each with a wireframe shell and a faint translucent face fill. Their colors slowly breathe through the hue spectrum.

Three rings of connecting line segments link vertices between the shells, rotating at different rates. 280 node particles orbit spherically around the structure. A pulsing white bloom at the center expands and contracts rhythmically. The camera orbits slowly and drifts up and down on a gentle sine wave, with mouse or finger movement nudging your viewing angle.

A **Spiral** toggle sits in the bottom-right corner. When enabled, the camera slowly spirals inward from its orbit radius over 60 seconds — pulling you deep inside the nested geometry — then releases back out over the next 60 seconds. Defaults to off.

### Desert Night
You drift slowly over a moonlit desert landscape. A full moon with a soft glow halo sits high in the sky, casting a cool blue-silver wash across the entire scene. Rolling dune silhouettes line the horizon, each with a thin bright ridge highlight catching the moonlight along its crest. Saguaro cacti with branching arms and angular rock formations provide landmarks and scale. A subtle heat shimmer band ripples at the horizon. The Milky Way-style starfield twinkles continuously. Shooting stars streak across the sky every 5–12 seconds. Fine dust drifts in a slow desert wind.

**Desert wildlife** crosses the scene occasionally, each with a distinct silhouette and movement style:
- **Roadrunner** — darts quickly across, legs alternating in a run, head bobbing, tail angled upward
- **Quail** — a covey of 4–7 birds crosses slowly together, each with an iconic topknot plume that sways as they walk
- **Gila Monster** — crawls deliberately slow, segmented body undulating, four splayed legs shuffling
- **Coyote** — trots across at medium speed, occasionally pausing, long tail drooping with a tuft at the end
- **Javelina** — a group of 2–3 stocky peccaries shuffle together, wide flat snouts, bristly ridge along the back

Mouse or finger movement tilts your view across the landscape.

### Thunderstorm
You drift slowly over a dark landscape as a massive storm rolls overhead. Three depth layers of volumetric clouds — far (wide, diffuse), mid, and near (darker, sharper) — drift at different speeds creating genuine parallax depth. Each cloud is built from three overlapping planes for added volume.

Lightning bolts are jagged 14-segment strikes with a secondary branch splitting off the midpoint. Each strike triggers a strong flash that illuminates the clouds from within, with a secondary flicker 80ms later. Distant horizon lightning flares inside the far clouds every few seconds — no bolt visible, just the storm lit from deep within. Ground puddle reflections shimmer at ground level and briefly brighten with each flash. Rain streams down at a wind angle, with squalls that surge intensity every 7–12 seconds before easing back. Wind-blown debris particles cross the scene horizontally.

A **Storm** toggle sits in the bottom-right corner. When enabled, lightning strikes every 2–6 seconds. Toggle it off for infrequent lightning every 12–18 seconds — a calmer, distant storm feel. Switching immediately resets all lightning timers to the new interval.

Mouse or finger movement tilts your view across the landscape.

---

## Controls

| Input | Effect |
|-------|--------|
| **Mode buttons** | Bottom center pill — switches between the six scenes with a fade transition |
| **Pulse toggle** | Bottom right — Warp mode only, enables/disables speed surges |
| **Spiral toggle** | Bottom right — Sacred Geometry mode only, enables/disables the inward camera spiral |
| **Storm toggle** | Bottom right — Thunderstorm mode only, switches between heavy and calm lightning |
| **Fullscreen button** | Top right — enters/exits fullscreen mode |
| **Mouse move / finger drag** | Subtly influences every scene |

UI and toggles auto-hide after 3.5 seconds of inactivity and reappear on any mouse movement or tap.

---

## Device Support

- **Desktop** — full experience with mouse interaction and custom cursor
- **Mobile & tablet** — full touch support; drag a finger to influence each scene, tap to reveal the UI. The custom cursor is hidden automatically on touch devices.
- Works in Chrome, Safari, Firefox, and Edge on both desktop and mobile

---

## Technical Notes

- Built with [Three.js](https://threejs.org/) (r128) and vanilla JavaScript
- Single `index.html` — no build step, no dependencies to install
- Frame rate capped at 30fps; full memory cleanup on every scene switch
- Designed to run for 1+ hours without degradation
- Hosted via GitHub Pages (static, always-on, no cold starts)
