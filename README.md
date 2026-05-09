# Autonomous-Drone 
Autonomous drone navigation system featuring A*, RRT & RRT* path planning (Simulink/Stateflow) and a Python computer vision stack with gesture control, body following, jump detection, and line following.

## 📁 Structure

```
├── Matlab Model/        # A*, RRT, RRT* in Simulink/Stateflow
│   └── benchmarks/       # Results across obstacle maps
└── pysim/                # Python drone simulation (Pysimverse)
```

---

## 🗺️ Path Planning — Simulink / Stateflow

Three algorithms implemented and benchmarked across obstacle maps:

| Algorithm | Type | Notes |
|-----------|------|-------|
| **A\***   | Graph-based | Optimal, heuristic-guided |
| **RRT**   | Sampling-based | Probabilistically complete |
| **RRT\*** | Sampling-based | Asymptotically optimal |

Benchmarks compare path length, computation time, and success rate across maps of varying obstacle density.

---

## 🐍 Python Simulation — Pysimverse

Drone simulation built with [Pysimverse](https://pysimverse.com/).

Missions covered:
- 3D movement, takeoff & landing
- Video streaming & image capture
- Hand gesture control (MediaPipe)
- Body following & jump detection
- Autonomous line following + PID control

---

## ⚙️ Setup

**Simulink** — MATLAB R2023b+ with Simulink and Stateflow toolboxes.

**Python sim:**
```bash
pip install pysimverse
python pysim/main.py
```
Requires Python 3.13+ and Pysimverse installed from [pysimverse.com](https://pysimverse.com/).
