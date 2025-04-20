# ECCV: Enhanced Clustering using Conditional Volatility

This repository contains the source code, data, and supporting materials for the research framework **ECCV (Enhanced Clustering using Conditional Volatility)** for clustering time-series data, including both benchmark and real-world Thai stock market datasets.

---

## 🔍 Project Structure


---

## 📁 benchmark/

- `A_Benchmark_study_ARIMA_GARCH.ipynb`  
   → Code for building ARIMA-GARCH models to estimate conditional volatility on benchmark data.
- `A_Benchmark_study_Clustering.ipynb`  
   → Code for running clustering algorithms (KMeans, Spectral, CLARA, etc.) on CV data.
- `A_Benchmark_study_TS_dataset_source.txt`  
   → UCR dataset links used for benchmarking.
- `Statistics_test.ipynb`  
   → Statistical test for normality and variance to enhance clustering accuracy.

---

## 📁 real_world/

- `Real_world_Thai_stock_data.ipynb`  
   → Full workflow for real Thai stock data: data cleaning, ARIMA-GARCH modeling, CV extraction, clustering.
- `Adj_price_stock_raw_data.csv`  
   → Adjusted closing price from Yahoo Finance for Thai stocks.
- `Best_ARIMA_Model.csv`  
   → Selected ARIMA models with AIC and performance stats.
- `Best_GARCH_Model.csv`  
   → GARCH modeling results for volatility estimation.
- `Conditional_volatility_data.csv`  
   → Estimated CV from best GARCH models for each stock.
- `Seasonal_test.csv`  
   → Results of seasonal stationarity testing (ADF, LBQ).

---

## 📊 Framework Diagram

![ECCV Framework](images/ECCV_framework_diagram.png)

---

## 📦 How to Use

1. Install Jupyter Notebook/Colab environment
2. Run notebooks under `benchmark/` and `real_world/` folders
3. Make sure to install required packages (e.g., `arch`, `pmdarima`, `scikit-learn`, `tslearn`)
Note-Run the code step by step, some parts require loading files from CSV or others.
---

## 📎 Citation & Appendix Link

This GitHub repository is referenced in the Appendix of the thesis.  
📎 **Appendix Link**: [https://github.com/Prakarn-Taranodom/ECCV-framework-clustering](https://github.com/Prakarn-Taranodom/ECCV-framework-clustering)

