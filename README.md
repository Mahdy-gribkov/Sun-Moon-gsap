# Sun & Moon — 3D GSAP Animations

Interactive 3D sun and moon scenes with shader-based effects, mouse tracking, and orbital animations.

Built with **GSAP** and **Three.js**.

[View on CodePen](https://codepen.io/mahdy-gribkov)

---

## Scenes

| Scene | File | Features |
|---|---|---|
| **Sun** | `sun.html` | Pulsing shader glow, orbital elements, mouse-following |
| **Sun (Blink)** | `sun_blink.html` | Above + reactive facial animations |
| **Moon** | `moon/` | Lunar variation with adjusted palette |
| **Moon (Blink)** | `moon-blink/` | Moon + interactive expressions |
| **Sun (CodePen)** | `sun-code-pen/` | Optimized version for CodePen |

## How It Works

- **Shader uniforms** drive the pulsing glow effect with GSAP's `yoyo` and `sine.inOut` easing
- **Mouse tracking** with damped `power2.out` easing for smooth, natural following
- **Three.js groups** separate body, orbital elements, and facial features for independent animation
- **`onUpdate` callbacks** synchronize dependent properties (halo opacity scales with pulse)

## Run Locally

Just open any `.html` file in a browser. No build step required — all dependencies load via CDN.

```
# Example
open sun.html
```

## Tech Stack

| | |
|---|---|
| **Animation** | GSAP 3 |
| **3D** | Three.js |
| **Shaders** | Custom GLSL uniforms |
| **Interaction** | Mouse position tracking |

## License

MIT
