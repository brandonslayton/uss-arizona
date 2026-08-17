# USS Arizona — low-poly Three.js

Cartoon Constitution-class starship (named **ARIZONA**) in a single-file Three.js scene. Black space + starfield. Orbit to inspect.

**Live:** https://uss-arizona.vercel.app

## Run locally

Open `index.html` via a static server (ES modules). From this folder:

```bash
python -m http.server 8787
```

Then visit http://127.0.0.1:8787/

`enterprise.html` is the same file as `index.html`.

## Layout (for editors)

| File | Role |
|---|---|
| `index.html` | Full scene: ship group `enterprise`, lights, stars |
| `vercel.json` | Static deploy |
| `grok-image-*.jpg` | Reference plates (front / ¾ / side / top / aft) |

Ship is `window.enterprise` (`THREE.Group`). Coords: **+Z aft, −Z bow, +Y up, +X starboard**.

Keep it **low-poly and cartoony** (flatShading, no textures, no high-seg spheres). Match the reference JPGs for silhouette.

## Deploy

Pushed to Vercel project `uss-arizona` (team Slaytong).
