# 🌌 Repo Universe

> Explore any GitHub repository as an interactive 3D space — fly through nodes, warp between files, watch commits and releases float in orbit.

**[▶ Live Demo → dev0root6.github.io/git-network](https://dev0root6.github.io/git-network/)**

---

## What is this?

Repo Universe turns a GitHub repo into a navigable 3D node graph. Every folder, file, commit, and release becomes a glowing node scattered across deep space. You fly through it like a first-person game.

Paste any public GitHub URL → the entire repo tree is fetched live from the GitHub API → spawned as a 3D network you can explore.

---

## Features

- **3D node graph** — every file and folder scattered across full XYZ space, connected by glowing edges
- **Free-fly camera** — WASD to move, mouse to look, Space/Shift for vertical, scroll to adjust speed
- **Warp jump** — double-click any node to teleport directly to it with smooth easing
- **Gravity system** — nodes slowly drift and wander with soft anchors, edges update in real time
- **Node trails** — glowing trail follows your flight path through the graph
- **Pulse animation** — nodes breathe; file node size scales with actual file size
- **Commit cluster** — last 15 commits fetched and spawned as their own node cloud
- **Release cluster** — all releases with tag, notes, and download count
- **Tree index panel** — full indented file tree on the left, click any entry to warp there
- **Procedural textures** — canvas-generated noise textures on every directory sphere
- **Volumetric nebulae** — layered smoky clouds in the background using additive blending
- **Multi-layer starfield** — 3 depth layers + milky way band
- **Mobile joysticks** — dual virtual joysticks on touch devices, left to move, right to look
- **Animated intro** — live 2D canvas intro with floating nodes and example repos

---

## Usage

### Online
Open **[dev0root6.github.io/git-network](https://dev0root6.github.io/git-network/)** in any browser.

### Local
```bash
# Clone or download repo-universe-v3.html
# Start a local server (required for GitHub API CORS)
python3 -m http.server 8080

# Open in browser
http://localhost:8080/repo-universe-v3.html
```

> **Note:** Must be served over `http://` — opening as `file://` will block GitHub API calls due to CORS.

---

## Controls

| Input | Action |
|---|---|
| `W A S D` | Fly forward / left / back / right |
| `Mouse` | Look around (click canvas to lock) |
| `Space` | Fly up |
| `Shift` | Fly down |
| `Scroll` | Adjust movement speed |
| `Double-click node` | Warp jump to node |
| `Click node` | Open info panel |
| `ESC` | Release mouse pointer |

### Mobile
| Input | Action |
|---|---|
| Left joystick | Move |
| Right joystick | Look |
| ▲ / ▼ buttons | Fly up / down |
| Tap node | Open info panel |

---

## Node types

| Color | Type |
|---|---|
| 🟡 Yellow | Root / repo |
| 🔵 Purple | Directory |
| 🔵 Cyan | File |
| 🟡 Amber | Commit |
| 🟢 Teal | Release |

---

## Stack

- [Three.js r128](https://threejs.org/) — 3D rendering
- GitHub REST API — live repo data
- Vanilla JS / HTML / CSS — no build step, single file

---

## Built by

[@dev0root](https://github.com/dev0root6) — pentester, hardware hacker, builder of things.

---

*This is an experiment. Not affiliated with GitHub.*
