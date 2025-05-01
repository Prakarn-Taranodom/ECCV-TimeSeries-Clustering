# ECCV: Enhanced Clustering using Conditional Volatility

This repository contains the source code, data, and supporting materials for the research framework **ECCV (Enhanced Clustering using Conditional Volatility)** for clustering time-series data, including both benchmark and real-world Thai stock market datasets.

---

## 🔍 Project Structure

This project is organized into two main parts:

- `benchmark/`: Analysis using synthetic datasets from UCR archive
- `real_world/`: Analysis using Thai stock market data
- `images/`: Framework diagram and visual assets

---

## 📁 benchmark/

- `A_Benchmark_study_ARIMA_GARCH.ipynb`  
   → Code for building ARIMA-GARCH models to estimate conditional volatility on benchmark datasets.
- `A_Benchmark_study_Clustering.ipynb`  
   → Code for running clustering algorithms (KMeans, Spectral, CLARA, etc.) using CV as features.
- `A_Benchmark_study_TS_dataset_source.txt`  
   → UCR dataset links used for benchmarking.
- `Statistics_test.ipynb`  
   → Statistical tests (e.g., normality, variance) to enhance clustering performance.
- `RandIndex_NMI_Result.csv`  
   → Clustering evaluation metrics (Rand Index, Normalized Mutual Information) for all methods.

📊 Meta-Feature Summary Files

- `Meta_type_summary_statistics.csv`
→ Summary statistics of key meta-features (e.g., ACF Lag-1, stationarity ratio, mean, std) grouped by dataset type. Useful for identifying structural patterns and comparing clustering performance across domains.

- `Meta_datasets_statistics.csv`
→ Dataset-level summary of meta-features for each benchmark dataset, including autocorrelation, stationarity, variability, and skewness metrics. Used for type-level and dataset-level analysis.

- `Meta_type_difference_summary.csv`
→ Difference in meta-feature values (Δ ACF Lag-1, Δ stationarity ratio) before and after applying CV, grouped by dataset type. This helps analyze how CV transformation structurally alters each data type.

---

## 📁 real_world/

- `Real_world_Thai_stock_data.ipynb`  
   → Full pipeline: data cleaning, ARIMA-GARCH modeling, CV extraction, and clustering on Thai stock data.
- `Adj_price_stock_raw_data.csv`  
   → Adjusted closing prices from Yahoo Finance for listed Thai companies.
- `Best_ARIMA_Model.csv`  
   → Summary of best ARIMA models with AIC and related parameters.
- `Best_GARCH_Model.csv`  
   → Summary of best GARCH models for each stock.
- `Conditional_volatility_data.csv`  
   → Conditional Volatility (CV) matrix generated from GARCH modeling.
- `Seasonal_test.csv`  
   → Results of seasonal tests (ADF, LBQ, etc.) for stationarity.
- `Thai_Stock_Sector.csv`  
   → Sector and industry labels for each stock, used in post-clustering analysis.

---

## 📊 Framework Diagram

![ECCV Framework](images/ECCV_framework_diagram.png)

---

## 📦 How to Use

1. **Install environment**:
   - Use Jupyter or Google Colab
   - (Optional) Set up virtual environment with:
     ```bash
     pip install -r requirements.txt
     ```

2. **Run Notebooks**:
   - Benchmark studies: navigate to `benchmark/`
   - Real-world Thai stock study: navigate to `real_world/`

3. **Google Colab Note**:
   - Mount Google Drive before accessing files
   - You may need to change file paths (e.g., `/content/drive/MyDrive/...`)

---

## 📎 Citation & Appendix Link

This GitHub repository is cited in Appendix A of the thesis.  
📎 **Appendix Link**: [https://github.com/Prakarn-Taranodom/ECCV-TimeSeries-Clustering](https://github.com/Prakarn-Taranodom/ECCV-TimeSeries-Clustering)

