# I-X Technical Tutorials: Bayesian Kinetics
 
This tutorial introduces Bayesian statistical modelling using PyMC for analysing enzyme kinetics in bioprocess development.

## 🚀 Overview

You will explore how to:
- Simulate kinetic data with latent effects (e.g. temperature, pH)
- Build Bayesian models to fit kinetic curves
- Extend models with Gaussian process (GP) priors for hybrid modelling

---

## 📁 Tutorial Structure

| Notebook | Title | Description |
|---------|-------|-------------|
| `0_data_generation.ipynb` | **[Hidden] Data generation** | ⚠️ *Not for initial use.* This notebook simulates the kinetic dataset. Use it only if you want to inspect or regenerate the synthetic data. |
| `1_bayesian_kinetics_intro.ipynb` | **Basic Bayesian model with mechanistic equation** | 🧪 Your starting point. Fit a simple model to the observed kinetic data using PyMC. |
| `2.1_bayesian_kinetics_gp_exercise.ipynb` | **Hybrid modelling with latent GP (Exercise)** | 🔬 Advanced model using a GP prior to capture latent dependencies (temperature/pH effects). |
| `2.2_SOLUTION_bayesian_kinetics_gp_exercise.ipynb.` | **Hybrid modelling with latent GP (Solution)** | 💡  The full solution in case you need help. |

---

## ✅ Start Here

Start with notebook 1:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lhelleckes/bayesian-kinetics-tutorial/blob/main/1_bayesian_kinetics_intro.ipynb)

Then explore hybrid modeling with GPs:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lhelleckes/bayesian-kinetics-tutorial/blob/main/2.1_bayesian_kinetics_gp_exercise.ipynb)

---

## 📦 Requirements

The easiest way to use the notebooks is via Google Colab.  
If running locally, install the dependencies via:

```bash
conda create -c conda-forge -n pymc_env "pymc>=5"
conda activate pymc_env
pip install pandas matplotlib
