🌍 Aerosol-Type Classification System

A Machine Learning–based Global Aerosol Identification Project

📌 Overview

This project focuses on building a complete aerosol-type classification system using optical properties and machine learning.
We classify aerosols into:

🟫 Dust

🟤 Mixed-Coarse

🟡 Mixed-Fine

🔵 Urban/Industrial

🔥 Biomass Burning

Our system integrates data preprocessing, feature extraction, optical modeling, and a Random Forest classifier to accurately identify global aerosol types from AERONET optical data.

👥 Team Members

Karan Khonde

[Add other group members]

🚀 Features

✔ Classifies aerosols into 5 categories
✔ Uses AERONET optical parameters (SSA, AOD, EAE, g)
✔ Includes optical simulation using the Mie Scattering model
✔ Robust Random Forest classifier for final predictions
✔ Global aerosol-type distribution visualization
✔ Clean and modular code structure

🧠 System Architecture

Our aerosol classification pipeline consists of four main modules:

1. Data Preprocessing

Reads raw AERONET Level-2 data

Removes invalid/noisy readings

Normalizes optical parameters

2. Feature Engineering

Extracts core features:

Single Scattering Albedo (SSA)

Ångström Exponent (EAE)

Normalized AOD

Asymmetry parameter (g)

3. Optical Modeling

Uses Mie Scattering to simulate optical behavior

Generates additional features based on:

Particle size distribution

Refractive index

Wavelength-dependent absorption/scattering

4. Machine Learning Model

Random Forest Classifier

Hyperparameter tuning using Grid Search

Outputs 5 aerosol-type labels

📊 Dataset

We used global AERONET data covering multiple regions:
Africa • Asia • Europe • North America • South America

Each region includes diverse aerosol sources such as desert dust, urban pollution, and biomass burning.

📈 Model Performance

Accuracy: ~89%

Micro Precision: ~95%

Micro Recall: ~89%

Micro F1-Score: ~91%

The system performs strongly across all aerosol categories, especially Dust, U/I, and Biomass Burning.

🛠 Tech Stack

Python

NumPy / Pandas

Scikit-learn

Matplotlib

Mie Scattering Simulation Library

AERONET Dataset

📁 Project Structure
├── data/
│   ├── raw/
│   ├── processed/
├── src/
│   ├── preprocess.py
│   ├── feature_engineering.py
│   ├── mie_scattering.py
│   ├── classify.py
│   ├── model.py
│   ├── visualization.py
├── results/
│   ├── plots/
│   ├── maps/
├── README.md
├── requirements.txt

▶️ Usage
1. Install Dependencies
pip install -r requirements.txt

2. Preprocess Dataset
python src/preprocess.py

3. Generate Optical Features
python src/feature_engineering.py

4. Train the Classifier
python src/model.py

5. Classify New Aerosol Data
python src/classify.py --input sample.csv

🌐 Visualizations

The project includes:

Aerosol-type pie charts

Continental distribution maps

Confusion matrix of model performance

SSA vs EAE clusters

Global aerosol-type map

🤝 Contribution

Pull requests and improvements are welcome.
To contribute:

Fork the repo

Create a new branch

Commit changes

Submit a PR

📄 License

This project is open-source under the MIT License.
