# 🏠 Housing and Social Inequality in Ireland  
### K-Means Clustering on Census 2022 Data

## 📌 Project Summary

Machine learning project analysing housing pressure and socio-economic inequality across Ireland using K-Means clustering.

Focuses on uncovering hidden territorial patterns beyond traditional urban–rural classifications.

---

## 🛠️ Technologies

Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn · Jupyter

---

## 📊 Key Results

- Identified **4 socio-economic clusters**
- Revealed inequalities not captured by official classifications
- Highlighted housing pressure beyond urban areas

---

## 📊 Visualisations

### 🔹 1. Exploratory Data Analysis (EDA)

#### Distribution of key variables
![EDA Distribution](images/1_eda_distribution.png)

#### Overcrowding by original classification
![EDA Overcrowding](images/2_eda_overcrowding.png)

---

### 🔹 2. Model Selection

#### Elbow Method
![Elbow Method](images/3_elbow_method.png)

---

### 🔹 3. Clustering Results

#### Cluster formation
![K-Means Clusters](images/4_kmeans_clusters.png)

#### Cluster distribution
![Cluster Distribution](images/5_cluster_distribution.png)

---

### 🔹 4. Interpretation

#### Overcrowding by cluster
![Overcrowding by Cluster](images/6_overcrowding_by_cluster.png)

#### Original vs ML clusters
![Original vs Clusters](images/7_original_vs_clusters.png)

---

### 🔹 5. Feature Relationships

#### Feature scatter
![Feature Scatter](images/8_feature_scatter.png)

#### Cluster heatmap
![Cluster Heatmap](images/9_heatmap_clusters.png)

---

## ▶️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/Granades/housing-inequality-ireland-ml.git
cd housing-inequality-ireland-ml

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Granades/housing-inequality-ireland-ml.git
cd housing-inequality-ireland-ml

### 2. Install dependencies

pip install pandas numpy scikit-learn matplotlib seaborn jupyter

### 3. Run the notebook

jupyter notebook
