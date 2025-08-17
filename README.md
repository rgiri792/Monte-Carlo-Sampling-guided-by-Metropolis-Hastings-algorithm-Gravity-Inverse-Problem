# 🪐 Monte Carlo Simulation for Gravity Inverse Problem  

This repository contains a **Jupyter Notebook** implementing a **Monte Carlo approach** to solve the **Gravity Inverse Problem**. The inverse problem aims to infer subsurface mass distributions from gravitational field measurements. Using randomized sampling and statistical inference, the method provides an approximate solution where deterministic inversion methods are difficult to apply.  

---

## 📌 Project Description  

The gravity inverse problem is a classic ill-posed problem in geophysics: given gravitational anomaly measurements at the surface, estimate the density distribution of subsurface bodies. Direct inversion is challenging due to **non-uniqueness** and **sensitivity to noise**.  

This project explores a **Monte Carlo simulation framework** for the inverse problem. Instead of seeking a single deterministic solution, the method evaluates a large number of randomly generated models and identifies those that best match the observed data.  

### Workflow:  
1. **Forward Gravity Model**  
   - Computes gravitational anomalies from a given subsurface mass distribution.  
2. **Monte Carlo Sampling**  
   - Randomly generates candidate subsurface models (density, depth, geometry).  
3. **Error/Objective Function**  
   - Calculates the misfit between observed and modeled gravitational data.  
4. **Model Selection**  
   - Retains models with the lowest error, representing possible solutions.  
5. **Statistical Analysis**  
   - Aggregates selected models to provide probabilistic estimates of subsurface properties.  

### Key Insights:  
- Monte Carlo methods provide a **probabilistic inversion** rather than a single solution.  
- Useful for quantifying **uncertainty** in subsurface density estimation.  
- Can reveal likely regions of mass anomalies even with noisy data.  

Applications include:  
- Geophysical exploration (oil, gas, minerals)  
- Subsurface structure identification  
- Earth and planetary science research  

---

## ⚙️ Features  
- Implementation of gravity forward modeling  
- Monte Carlo-based inversion strategy  
- Misfit/error calculation for model evaluation  
- Visualization of convergence and accepted models  
- Provides probabilistic rather than deterministic inversion results  

---

## 🔧 Requirements  
Ensure you have the following Python libraries installed:  
```txt
numpy  
matplotlib 
git clone https://github.com/<your-username>/MonteCarlo-Gravity-Inverse.git
cd MonteCarlo-Gravity-Inverse
jupyter notebook Monte_Carlo_Gravity_Inverse_Problem_V2.ipynb
 
scipy  
jupyter  
