# Building Water Pipeline Optimization with Simulated Annealing

## 📌 Description
This project implements the **Simulated Annealing** algorithm to optimize the selection of pipe diameters in a fluid flow system. The goal is to minimize costs while meeting velocity and pressure loss constraints.

## 🚀 Features
- Cost optimization for selecting pipe diameters.
- Uses the **Simulated Annealing** algorithm to find optimal solutions.
- Calculates fluid velocity, Reynolds number, and friction factor.
- Adjusts to available commercial diameters.
- Evaluates execution time, CPU usage, and memory consumption.
- Components: embodied carbon, pipe lifespan, pipe ease of installation, pipe ease of recycling, and pipe max work pressure.
  
## 📂 Project Structure
```
📁 pipeline_optimization
│── 📄 Cold-Water System_Raw Data.txt   # Sample water network data
│── 📄 Code.py   # Main code
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
python Code.py
```

The program will display:
- **Optimal diameter** and the **closest commercial diameter**.
- **Minimum cost** of the pipeline.
- **Fluid velocity** in each pipe.
- **Pressure loss**.
- **Total execution time**, **CPU** usage, and **memory** usage.
- **Hidden digital signature verification**.

## 🔧 Simulated Annealing Function
The function `simulated_annealing` contains the following parameters:

```python
def simulated_annealing(
    d_min, d_max, temp, cooling_rate, max_iter, C, l, E_p, I_p, L_p, R_p, P_p, n_no_improvement=500
):
```
- `d_min`, `d_max`: Range of possible diameters.
- `temp`: Initial temperature.
- `cooling_rate`: Cooling rate per iteration.
- `max_iter`: Maximum number of iterations.
- `C`, `l`: Cost parameters and pipeline lengths.
- `E_p`, `I_p`, `L_p`, `R_p`, `P_p`: Penalty factors for constraints.
- `n_no_improvement`: Number of iterations without improvement before stopping.

### **Returns:**
- `best_d`: Optimized diameters.
- `best_cost`: Minimum cost found.
- `total_time`: Total execution time.
- `cpu_used`: CPU processing time used.
- `memory_used`: Memory consumption in MB.
- `actual_iterations`: Number of real iterations performed.
- `cost_history`: Cost values at each iteration.

## 👤 Author
**Pedro Maximiliano Cortez Lara, Benjamin Sanchez Andrade, and Hector Alfonso Barrios Piña** - 2025.

If you use this code, give me credit or send improvements! 😊
