# Human3D Models

A static gallery of **3D human character models** (GLB / FBX) for use with Three.js or other WebGL runtimes.

![Three.js](https://img.shields.io/badge/Three.js-Ready-000000?style=flat-square&logo=threedotjs&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-222222?style=flat-square&logo=github&logoColor=white)

## Contents

| File | Format | Description |
|------|--------|-------------|
| `models/StandingIdle.glb` | GLB | Standing idle pose |
| `models/StandingPerson.fbx` | FBX | Standing person mesh |

## Usage

### Local

Open `index.html` in a browser, or serve statically:

```bash
python3 -m http.server 8080
```

### GitHub Pages

`.nojekyll` is included — enable Pages on the `main` branch and point your Three.js app at the raw model URLs.

## Integrating with Three.js

```javascript
import { GLTFLoader } from 'three/examples/jsm/loaders/GLTFLoader.js';

const loader = new GLTFLoader();
loader.load('models/StandingIdle.glb', (gltf) => {
  scene.add(gltf.scene);
});
```

---

[malimba](https://github.com/malimba)
