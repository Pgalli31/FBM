# Fractional Brownian Motion & Financial Simulation

This project explores the concept of **Fractional Brownian Motion (FBM)** and its associated **Fractional Gaussian Noise (FGN)** to simulate and visualize time-series data. The project applies these models to understand persistent and anti-persistent behavior in stock price trends using different generation methods.

## 📘 Overview

Fractional Brownian Motion (FBM) is a generalization of classical Brownian Motion that introduces long-term memory or persistence through the **Hurst exponent (H)**:
- **H < 0.5**: Anti-persistent behavior (reversing trends)
- **H = 0.5**: Classical Brownian motion
- **H > 0.5**: Persistent behavior (trending)

FGN is the increment process of FBM and captures similar behavior in discrete steps.

## 🧪 Methods

The project simulates FBM and FGN using the following methods:
- **Hosking** – recursive and memory-efficient
- **Cholesky** – accurate but memory-intensive
- **Davies-Harte** – fast and efficient using FFT

Libraries used:
- `fbm`
- `numpy`
- `matplotlib`

## 📊 Visualizations

The project generates 24 graphs showing FBM and FGN behavior under:
- 4 Hurst values (0.2, 0.4, 0.6, 0.8)
- 3 simulation methods (Hosking, Cholesky, Davies-Harte)

Comparison plots are also generated between real Apple stock data and simulated data to evaluate trend alignment.

## 📈 Application to Finance

By aligning FBM/FGN simulations to real-world Apple stock log returns, this project demonstrates:
- The effect of persistence on price behavior
- The potential of FBM in generating synthetic financial data for modeling when historical data is limited

## 📁 Files

- `fbm_simulation.py` – Script to generate FBM/FGN samples
- `visualizations/` – Folder containing all generated graphs
- `apple_stock_comparison.py` – Code comparing FBM to actual stock data

## 🧠 Conclusion

FBM and FGN are useful tools for simulating time-series data that incorporates memory. They are especially valuable in fields like:
- Finance (e.g., stock modeling)
- Climate modeling
- Biomedical signals
- Internet traffic analysis

---

### 🔧 Future Work
- Extend to Geometric FBM for stock price simulation
- Incorporate real financial indicators for hybrid models
- Build an interactive dashboard to adjust H, method, and view real-time simulations

---

**Author:** Paul Galli  
