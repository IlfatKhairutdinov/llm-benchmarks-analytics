# LLM Benchmarks & Investment Efficiency (2020-2026)
### Exploratory Data Analysis (EDA), Advanced Data Cleaning & Predictive ML Modeling

---

## 📌 Executive Summary
This production-ready Data Science project delivers a comprehensive Exploratory Data Analysis (EDA) and predictive modeling pipeline of the global LLM ecosystem spanning from 2020 to 2026. By merging heterogeneous data files—combining multi-source evaluation benchmarks with estimated compute expenditures—this pipeline maps the Pareto-efficiency of language models. 

Using Unsupervised Learning (PCA) and Supervised ML (Linear Regression), the project successfully uncovers hidden structural clusters in the market and forecasts the growth vector of generative AI capabilities up to December 31, 2026.

---

## 🧠 Core Engineering Practices Demonstrated
* **Secure API Integration:** Complete decoupling of credentials using Google Colab's native `userdata` Secrets architecture. Zero hardcoded tokens, ensuring maximum security for GitHub deployment.
* **Algorithmic Data Aggregation:** Robust handling of multi-file structures via dynamic pandas key-matching and automated Cartesian product mitigation (`drop_duplicates`).
* **Heuristic Outlier & Corruption Filtering:** Advanced feature engineering that programmatically isolates valid evaluation metrics (0-100% or 0-1000 scales) from high-magnitude technical IDs and raw parameter weights, preventing severe statistical skew.
* **Dimensionality Reduction (PCA):** Implementation of Unsupervised Learning (Principal Component Analysis) to compress a 17-dimensional benchmark matrix into 2 principal orthogonal components, mapping the entire LLM landscape on a 2D vector space.
* **Predictive ML Modeling & Data Transformation:** Built a Scikit-Learn Linear Regression pipeline with automated string-to-ordinal datetime transformation to forecast industry capability trajectories.

---

## 🛠️ Tech Stack & Dependencies
* **Core:** Python 3.10+, pandas, numpy
* **Machine Learning:** scikit-learn (StandardScaler, PCA, LinearRegression)
* **Infrastructure:** kagglehub (Secure Dataset Streaming)
* **Visualization:** plotly-express, seaborn, matplotlib

---

## 📈 Key Insights & Analytical Deliverables

### 1. Hard Data-Driven ML Forecast
The predictive regression pipeline establishes the industry-wide baseline growth vector. The model mathematically forecasts that by **December 31, 2026**, the average performance baseline across newly released LLM architectures will stabilize at **47.15%** across the comprehensive benchmark pool, reflecting the law of diminishing returns on compute scaling.

### 2. Latent Structure Mapping via PCA
Rather than analyzing 17 correlated heatmaps, the PCA component decomposition reveals hidden clusters of models. The top 2 principal components successfully capture 100.00% of the dataset's variance, clearly separating high-ROI open-weights architectures from capital-intensive proprietary monoliths based on latent cognitive traits.

### 3. The Training Cost vs. Capability Dilemma
By mapping `average_benchmark_score` against `training_cost_usd_est` on a logarithmic scale, the project explicitly identifies frontier models that disrupt proprietary monopolies on a cost-per-token and cost-to-train basis.

---

## 🚀 Quick Start (Google Colab Deployment)

1. **Configure Your Credentials securely:**
   In your Google Colab notebook, click the Secrets (Key icon) tab on the left panel and add:
   * `KAGGLE_USERNAME`: Your personal Kaggle identifier.
   * `KAGGLE_KEY`: Your dedicated Kaggle API token.
   * *Enable "Notebook Access" for both keys.*

2. **Run the Notebook:**
   Clone this repository directly into your environment or load the `.ipynb` file. The pipeline executes end-to-end autonomously—fetching files, cleaning anomalies, generating interactive PCA/Regression reports, and outputting the final 2026 capability forecast.

---

## 📬 Contact & Collaboration
Developed by an ambitious Data Scientist looking to build high-ROI ML systems. Feel free to fork, open an issue, or reach out via GitHub if you want to scale this project further!
