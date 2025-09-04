# 🧠 Optimal Park Placement Using QAOA

This project is a simple demonstration of using the **Quantum Approximate Optimization Algorithm (QAOA)** to solve a real-world inspired spatial problem: placing a park in a village to minimize walking distance from important buildings.

## 🏙 Problem Description

We simulate a small 3x2 grid village (6 cells total) with the following public facilities:

- 🏫 School: (0, 0)
- 🏛️ Village Committee: (2, 1)
- 👵 Senior Center: (0, 1)

**Goal:** Select a single cell to place a park such that the total distance from the park to all three facilities is minimized.

## 🧮 Optimization Strategy

- The grid is represented using 6 binary variables (1 for selected, 0 for not).
- We use **QUBO formulation** with:
  - Distance-based cost function
  - One-hot encoding constraint (only one cell can be selected)
- Solved using Qiskit's implementation of **QAOA** on a local quantum simulator.

## 🔧 Tech Stack

- Python 🐍
- Qiskit by IBM
- Matplotlib (optional)

## 🚀 How to Run

```bash
pip install qiskit matplotlib
python park_qaoa.py
```
## 📈 Example Output
Best location: cell 2 at coordinate (2, 0)
Total distance to facilities: 6
## 💡 Why QAOA?
This demo showcases how QAOA can be applied to real-world-style optimization problems involving spatial layouts, logistics, and planning — providing a great starting point for deeper quantum applications.

© 2025 Hope Alemayehu
