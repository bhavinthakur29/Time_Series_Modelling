# Oil Price Forecasting – ARIMA & LSTM (Time Series Case Study)

This repository contains the code for my university time series modelling assignment.  
The project focuses on forecasting daily oil prices using two different approaches:

- **ARIMA** (classical statistical model)
- **LSTM** (deep learning model)

The aim is to compare their performance, generate 24‑month forecasts, and evaluate how well the models generalise to unseen data.

This repo is intended both as part of my coursework submission and as a reference for anyone learning time series forecasting in Python.

---

## 📁 Repository Contents

```
├── notebook.ipynb          # Main Jupyter Notebook with full workflow
├── code.py                 # Exported .py version of the notebook
├── data/                   # Input dataset (oil prices 2024–2026)
├── figures/                # All plots saved automatically by the notebook
└── README.md               # Project overview (this file)
```

---

## 🚀 How to Run the Project

1. Install Python 3.10+  
2. Install the required libraries:

```bash
pip install numpy pandas matplotlib statsmodels scikit-learn tensorflow
```

3. Open the notebook:

```bash
jupyter notebook notebook.ipynb
```

4. Run all cells from top to bottom.  
All figures will be saved automatically in the `figures/` folder.

---

## 📊 Overview of the Models

### **ARIMA**
- Stationarity testing (ADF, KPSS)
- Differencing and ACF/PACF analysis
- Grid search over (p, d, q)
- Residual diagnostics
- Train/test evaluation
- 24‑month forecast with confidence intervals

### **LSTM**
- Sequence generation with lookback windows
- Normalisation without data leakage
- Stacked LSTM architecture with dropout
- Early stopping during training
- Hyperparameter tuning
- Monte Carlo dropout for uncertainty estimation
- 24‑month forecast with confidence intervals

---

## 📈 Figures

The notebook automatically saves all key plots, including:

- Raw series and rolling statistics  
- ACF/PACF plots  
- Differenced series  
- ARIMA residual diagnostics  
- Train/test performance for both models  
- 24‑month forecasts  
- ARIMA vs LSTM comparison  
- Forecast vs real post‑Feb 2026 prices  

These are stored in the `figures/` directory.

---

## 📝 Report

The full written report (methods, results, interpretation, and discussion) is submitted separately as part of the assignment.  
This repository focuses on the code and reproducibility of the modelling process.

---

## 📬 Author

**Bhavin Thakur**  
Student ID: 23079699  
London, United Kingdom