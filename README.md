# AAI-530 Final Team Project — Traffic Flow Forecasting (Group 1)

## Project Overview
This project uses the UCI *Traffic Flow Forecasting* dataset to build an IoT analytics pipeline for short-term traffic prediction. We clean and analyze roadway sensor data, train baseline and deep learning forecasting models, and communicate insights through an interactive Tableau dashboard. The project also includes a theoretical smart city IoT system design that contextualizes how the data could be collected, processed, and used in practice.

## Dataset
**Source:** UCI Machine Learning Repository — Traffic Flow Forecasting  
**What it contains:** Traffic volume measured every 15 minutes across multiple sensor locations, along with engineered time and roadway features.  
**Prediction target:** Traffic volume 15 minutes into the future (per dataset description).

> [(DATASET LINK)](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)

### Data Access
Due to file size, raw data is not stored in this repository.
1. Download the dataset from the UCI page.
2. Place files into: `data/raw/`
3. Run preprocessing to generate modeling datasets in: `data/processed/`

## Repository Structure
- `data/` — raw (instructions) and processed datasets  
- `notebooks/` — EDA, baseline modeling, deep learning modeling  
- `src/` — reusable preprocessing, modeling, and evaluation code  
- `docs/` — IoT system design + figures  
- `dashboard/` — Tableau Public link and notes  
- `reports/` — submitted PDFs (proposal, progress update, final report)

## Methods (Planned)
- **EDA & preprocessing:** missing value handling, timestamp parsing, feature checks
- **Baseline forecasting:** classical ML/time-series baseline (e.g., linear regression or ARIMA-style baseline)
- **Deep learning forecasting:** sequence model (LSTM/GRU) for short-term prediction
- **Additional analytics (optional):** clustering to identify traffic pattern types (weekday/weekend, high congestion days)

## Tableau Dashboard
Tableau Public link: (add link here when ready)

## How to Run (High-level)
1. Create environment and install requirements:
   ```bash
   pip install -r requirements.txt

2. Run notebooks in order:
- notebooks/01_eda.ipynb
- notebooks/02_baseline_models.ipynb
- notebooks/03_deep_learning.ipynb

## Team Roles
- **Ashley Marx**: Data engineering, EDA, feature engineering, baseline modeling, clustering.
- **Noslinn Tosta**: GitHub management, deep learning forecasting, IoT system design, integration support.
