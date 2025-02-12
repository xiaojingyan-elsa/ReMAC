# ReMAC
# ReMAC Simulation and Optimization

This repository contains a Python implementation for evaluating the performance of **ReMAC, ChannelComp, and Bit-Slicing** in the presence of fading channels. The script optimizes transmission schemes using **Mixed-Integer Quadratic Constrained Programming (MIQCP)** and evaluates function computations under noisy conditions.

## 📌 Features
- **Function Evaluation**: Computes sum, product, max, norm, and fraction-based functions for multi-user networks.
- **Optimization with Gurobi**: Solves MIQCP problems for optimal transmission schemes.
- **Singular Value Decomposition (SVD)**: Extracts principal components from the optimization matrix.
- **Monte Carlo Simulations**: Evaluates performance under varying noise conditions.
- **Noise Impact Analysis**: Plots **NMSE vs. Noise Variance** for different transmission slots.

## 📦 Requirements
Before running the script, install the necessary dependencies:

```bash
pip install numpy cvxpy gurobipy matplotlib
```

## ⚙️ Customization

You can modify the following parameters in the script to adapt it to different scenarios:

### 🔹 Function Selection
To choose a different function for evaluation, modify the `function_name` variable in the script:

```python
function_name = 'sum'  # Choose from 'sum', 'prod', 'max', 'norm'
```
### 🔹 Noise Settings
Adjust `std_dev_vector` to simulate different noise levels.

### 🔹 Number of Users/Time Slots
Modify `num_users` and `num_time_slots` for different scenarios.

## 📊 Results

The script generates a **log-scale NMSE plot** to compare the performance of **ReMAC, ChannelComp, and Bit-Slicing** under different noise conditions.

### 🔹 NMSE vs. Noise Variance
The **Normalized Mean Squared Error (NMSE)** is plotted against different noise variance levels to analyze the impact of fading and noise on computational accuracy.

- **X-axis**: Noise Variance
- **Y-axis**: NMSE (Log Scale)
- **Results**: Performance of ReMAC


