<div align="center">

# 🎵 Spotify 2014–2020 Data Science Portfolio Project

### A complete end-to-end data science analysis of Spotify tracks  
### featuring EDA, statistics, anomaly detection, time series, network analysis, clustering, and machine learning

<br>

<img src="https://img.shields.io/badge/Python-Data%20Science-1DB954?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Pandas-Analysis-141420?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/Scikit--Learn-ML-F97316?style=for-the-badge&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/Matplotlib-Visualization-4ECDC4?style=for-the-badge" />
<img src="https://img.shields.io/badge/NetworkX-Network%20Analysis-A855F7?style=for-the-badge" />

</div>

---

## 📌 Project Summary

This project is a **portfolio-level end-to-end data science case study** built on a Spotify dataset from **2014 to 2020**.  
It explores how track characteristics, naming patterns, collaborations, anomalies, and categories evolve over time.

The project combines:

- **Exploratory Data Analysis**
- **Statistical Testing**
- **Feature Engineering**
- **Anomaly Detection**
- **Time Series & Trend Analysis**
- **Artist Collaboration Network Analysis**
- **Clustering & PCA**
- **Machine Learning Classification**

The final result is a **multi-page visual analytics project** designed with a custom **Spotify-inspired dark theme**.

---

## 🎯 Project Goals

This project aims to answer questions such as:

- How did Spotify track characteristics change between **2014 and 2020**?
- Did track duration, collaborations, and naming complexity change over time?
- Which tracks behave like anomalies?
- Can tracks be grouped into meaningful clusters?
- Can we predict track categories using engineered features?
- What does the artist collaboration network reveal?

---

## 🗂 Dataset

**Dataset used:** `spotify_2014_2020_dataset.csv`

The dataset contains information such as:

- `Track_ID`
- `Track_Name`
- `Artists`
- `Duration_Min`
- `Release_Date`
- `Year`
- `Query`

---

## ⚙️ Tech Stack

### Programming Language
- **Python**

### Libraries
- **Data manipulation:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Statistics:** `scipy`
- **Machine learning:** `scikit-learn`
- **Network analysis:** `networkx`
- **Text processing:** `re`, `collections`

---

## 🧠 Feature Engineering

A major strength of this project is the feature engineering process.

### Engineered Features
- `Artist_Count`
- `Name_Length`
- `Word_Count`
- `Has_Feat`
- `Has_Remix`
- `Has_Number`
- `Has_Parenthesis`
- `Is_Collab`
- `Duration_Log`
- `Duration_Sq`
- `Artist_x_Dur`
- `Year_Norm`
- `Is_Summer`
- `Release_Month`
- `Release_Quarter`
- `Name_Entropy`
- `Query_Encoded`

These features were later used in:
- statistical analysis
- anomaly detection
- clustering
- classification models

---

# 📊 Project Sections

## 1️⃣ Exploratory Data Analysis
This section explores the dataset structure and descriptive patterns.

### Included analyses
- Track count per year
- Category distribution
- Duration histogram with fitted distributions
- Year × category percentage breakdown
- Violin plot of duration by category
- Collaboration and artist count trends
- Feature trend heatmap
- Top track-name words
- Ridgeline KDE plots by year

**Output:** `page1_eda.png`

---

## 2️⃣ Statistical Deep Dive
This section focuses on deeper statistical understanding of the data.

### Included analyses
- Full correlation matrix
- Shapiro-Wilk normality tests
- Q-Q plot for duration
- Box plots by year
- ANOVA p-values across category pairs
- KDE curves by category
- Duration vs. name entropy scatter analysis

**Output:** `page2_stats.png`

---

## 3️⃣ Anomaly Detection
This section detects unusual and outlier-like tracks.

### Methods used
- **Isolation Forest**
- **Local Outlier Factor (LOF)**

### Included analyses
- ISO score distribution
- LOF score distribution
- Overlap of anomaly detection methods
- Anomaly rate by year
- Scatter plots highlighting anomalies
- Top 20 most anomalous tracks

**Output:** `page3_anomaly.png`

---

## 4️⃣ Time Series & Trend Analysis
This section examines how Spotify-related patterns evolve across years.

### Included analyses
- Mean duration trend with forecast
- Collaboration / feat / remix trend analysis
- Artist count trend
- Cumulative growth and year-over-year change
- Name entropy trend
- Category-wise yearly trends
- Monthly release distribution
- Year × quarter release heatmap
- Word count forecast

**Output:** `page4_timeseries.png`

---

## 5️⃣ Artist Collaboration Network
This section creates a collaboration graph between artists.

### Metrics used
- Weighted degree
- Betweenness centrality
- Closeness centrality
- Density
- Average clustering coefficient
- Connected components

### Included analyses
- Artist collaboration network graph
- Top artists by weighted degree
- Top artists by betweenness centrality
- Network metrics summary
- Degree distribution

**Output:** `page5_network.png`

---

## 6️⃣ Clustering & Dimensionality Reduction
This section groups tracks into clusters and visualizes them.

### Methods used
- **StandardScaler**
- **K-Means**
- **PCA**

### Included analyses
- Elbow method
- PCA 2D cluster projection
- Explained variance
- Cluster profiles
- Cluster distribution by year
- Cluster × category heatmap
- Cluster size distribution

**Output:** `page6_clustering.png`

---

## 7️⃣ Machine Learning Classification
This section builds supervised learning models to classify track categories.

### Models used
- **Random Forest**
- **Gradient Boosting**
- **Logistic Regression**
- **Voting Ensemble**

### Included analyses
- Model comparison
- Confusion matrix
- Feature importance
- 10-fold cross-validation comparison
- PCA view of real categories
- Precision / Recall / F1 heatmap

**Output:** `page7_ml.png`

---

# 🚀 Project Outputs

The script generates the following visual dashboard pages:

```bash
page1_eda.png
page2_stats.png
page3_anomaly.png
page4_timeseries.png
page5_network.png
page6_clustering.png
page7_ml.png
