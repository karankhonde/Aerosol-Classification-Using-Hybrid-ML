# Global Aerosol Type Classification System

A machine learning-based hybrid algorithm for accurate classification of atmospheric aerosol types using AERONET data.

## 📋 Project Overview

This project implements an advanced aerosol classification system that combines Gaussian kernel density clustering, Mie scattering modeling, and random forest algorithms to identify five major aerosol types globally.

**Key Metrics:**
- 89% overall accuracy
- 95% micro-precision
- ~20 seconds processing time per site
- 47 AERONET sites across 5 continents

## 🎯 Objectives

- Develop a hybrid algorithm combining density clustering with machine learning
- Improve classification accuracy using multiple optical and microphysical parameters
- Create a scalable system for global aerosol monitoring
- Generate spatial distribution maps for climate research

## 🏗️ System Architecture

The system operates in three stages:

### Stage 1: Preliminary Classification
- Gaussian kernel density clustering on optical properties (SSA, EAE)
- Baseline characterization of five aerosol types

### Stage 2: Optical Database Generation
- Construct synthetic database using Mie scattering model
- Calculate complex refractive index (CRI) for each aerosol type
- Generate data at multiple wavelengths (440, 675, 870, 1020 nm)

### Stage 3: Classification & Validation
- Random forest classifier for aerosol identification
- Performance validation against baseline
- Global distribution mapping

## 📊 Aerosol Types Classified

1. **Dust Aerosols** - Desert-origin particles
2. **Mixed-Coarse** - Large particles with moderate absorption
3. **Mixed-Fine** - Small anthropogenic particles
4. **Urban/Industrial** - Fine particles from combustion
5. **Biomass Burning** - Particles from fires

## 🛠️ Tech Stack

- Python 3.7+
- scikit-learn (Random Forest, clustering)
- NumPy & Pandas (data processing)
- Matplotlib (visualization)
- Mie scattering library



## 📈 Performance Results

| Metric | Value |
|--------|-------|
| Overall Accuracy | 89% |
| Micro-Precision | 95% |
| Micro-Recall | 89% |
| Micro-F1-Score | 91% |


## 📊 Outputs

- Global and continental aerosol distribution maps
- Performance comparison visualizations
- Classification reports with regional statistics
- Interactive visualizations in Jupyter notebooks
