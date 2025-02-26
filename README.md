# Embodied-carbon-cost-and-size-analysis-for-optimal-water-network-design-in-buildings-
# Pipeline Optimization with Simulated Annealing

## 📌 Description
This project implements the **Simulated Annealing** algorithm to optimize the selection of pipe diameters in a fluid flow system. The goal is to minimize costs while meeting velocity and pressure loss constraints. Penalties are presented as function of environmental and techno-economic parameters to assess sustainable design. 

## 🚀 Features
- Cost optimization for selecting pipe diameters.
- Uses the **Simulated Annealing** algorithm to find optimal solutions.
- Calculates fluid velocity, Reynolds number, and friction factor.
- Adjusts to available commercial diameters.
- Evaluates execution time, CPU usage, and memory consumption.
- Penalties: embodied carbon, pipe lifespan, pipe ease of installation, pipe ease of recycling, and pipe max work pressure.

## 📂 Project Structure
```
📁 pipeline_optimization
│── 📄 main.py   # Main code
│── 📄 LICENSE   # Project license
│── 📄 README.md # This file
```

## 🛠 Installation & Requirements
This code requires **Python 3.x** and the following libraries:

```bash
pip install numpy psutil
```

## ▶️ Usage
Run the script with:

```bash
python main.py
```

The program will display:
- **Optimal diameter** and the **closest commercial diameter**.
- **Minimum cost** of the pipeline.
- **Fluid velocity** in each pipe.
- **Pressure loss**.
- **Total execution time**, **CPU** usage, and **memory** usage.

## 👤 Author
**Pedro Maximiliano Cortez Lara** - 2025.

If you use this code, give me credit or send improvements! 😊



