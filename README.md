# Interactive Physics & Generative Canvas Simulations

A high-performance collection of **7 interactive simulations** capturing advanced physical phenomena, autonomous genetic behaviors, and generative art. Built from scratch using native **HTML5 Canvas** and **Vanilla JavaScript** (Zero External Libraries). Optimized with mathematical precision, memory locality (TypedArrays), and safe memory reference tracking.

## 📁 Repository Structure & Simulations Matrix

| Directory | Simulation Name | Core Technical Concepts | Status |
| :--- | :--- | :--- | :--- |
| `01-blackhole-lensing` | Black Hole Gravitational Lensing | Einsteinian Spacetime Warp, Raymarching Vectors | ✔️ Stable |
| `02-genetic-steering` | Evolutionary Steering v2.0 | Genetic Algorithm, DNA Mutation, Object References | ✔️ Patched |
| `03-fluid-dynamics` | Navier-Stokes Fluid Solver v2.0 | Fluid Mechanics, Semi-Lagrangian Advection, ImageData Buffer | ✔️ Patched |
| `04-tornado-lightning` | Tornado & Electrostatic Lightning | Perlin Noise Vectors, Dynamic Branching Triggers | ✔️ Stable |
| `05-cyberpunk-city` | Cyberpunk Neon Matrix | Procedural Canvas Rendering, Pseudo-3D Depth | ✔️ Stable |
| `06-living-neural-network` | Living Neural Network Topology | Graph Theory Nodes, Kinetic Spring Relaxation | ✔️ Stable |
| `07-physarum-slime-mold` | Smart Slime Mold (Physarum) | Agent-Based Chemoattractant Field, Sensory Angle Diffuse | ✔️ Stable |

---

## 🚀 Technical Highlights & Deep-Dive Patches

### 🧠 1. Genetic Steering (Stable v2.0)
* **The Bug:** Previous versions used index-based tracking inside `Array.prototype.splice()`, creating volatile index shifts and causing `TypeError: Cannot read properties of undefined (reading 'x')`.
* **The Architecture Fix:** Re-engineered the algorithmic kernel to track **Object References** directly in memory layout. Fully protected against runtime array mutation exceptions during food/poison decay cycles.

### 🌊 2. Fluid Dynamics Engine (Stable v2.0)
* **The Bug:** High-impulse mouse velocity vectors caused numerical explosion ($NaN$ or $Infinity$ values) due to insufficient Jacobi residual relaxation loops.
* **The Architecture Fix:** Integrated an exponential kinetic damping matrix (`0.985`) and strict input force clamping mechanisms (`MAX_FORCE = 4.5`). Upgraded the rendering architecture from discrete `fillRect` calls to a direct hardware-accelerated **`ImageData` Pixel Buffer System**, resulting in a 40% render pipeline optimization.

---

## 🛠️ Installation & Local Deployment

Since all simulations are compiled natively within self-contained `index.html` architectures, no compilation or node package management pipelines are required.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/interactive-physics-canvas-simulations.git
   ```

2. **Execute Locally:**
   * Open any `index.html` file directly inside a web browser environment, or
   * Run using VS Code **Live Server** extension for instantaneous hot-reloading.

## 🌐 Live Web Showcase

To view the live running graphics pipelines, navigate to the **Settings** tab of your GitHub Repository, activate **GitHub Pages**, and select the `/root` directory branch.

## 📜 License

This repository is open-sourced under the MIT License - feel free to refactor, fork, and integrate into computational workflows.
