# ⚡ Smart Grid Energy Distribution Optimization using Genetic Algorithms

This project presents a parallelized solution to optimize energy distribution in a smart grid using Genetic Algorithms (GA). Designed for the **MLPC (Machine Learning & Parallel Computing)** course assignment, it tackles real-world constraints like fluctuating demand, transmission losses, and source capacity limits.

---

## 📌 Problem Statement

Efficient energy distribution in smart grids is a multi-objective, constrained optimization problem. The system must allocate power from multiple renewable sources (solar, hydro, wind) to multiple consumer nodes (residential/industrial) while minimizing:

- 🔸 Total operational cost  
- 🔸 Transmission losses  
- 🔸 Unmet demand  

Subject to constraints:
- Maximum generation capacity per source
- Hourly demand per node
- Non-negativity of allocated energy

---

## 🧠 Approach

This solution uses:
- **Genetic Algorithms (GA)** for optimization  
- **Parallelization (PyGAD + multi-threading)** to speed up computation  
- **Baseline algorithms** (Greedy & Rule-based) for benchmarking  
- **Data visualization** for performance insights  

---

## 🏗️ Architecture

- 📊 Synthetic data for 10 nodes × 24 hours
- ☀️ 3 energy sources: Solar, Hydro, Wind
- 📈 Fitness function combining cost, loss, deviation, and penalties
- 🔄 GA implementations:
  - **Serial GA**
  - **Parallel GA (4 threads)**
- 📊 Parameter sensitivity analysis on:
  - Population size
  - Mutation rate

---

## 🔍 Key Features

| Component          | Description                              |
|-------------------|------------------------------------------|
| 🧮 Fitness Function | Multi-objective: cost + loss + demand gap |
| 🧬 Genetic Algorithm | Customized with PyGAD (serial + parallel) |
| 📊 Visualizations   | Convergence, resource usage, energy heatmaps |
| ⚙️ Baselines        | Greedy and Rule-Based for comparison     |
| 📈 KPIs Tracked     | Runtime, fitness, loss, cost, speedup    |

---

## 📂 Repository Structure

