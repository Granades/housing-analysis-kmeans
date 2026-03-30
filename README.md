Machine learning project based on Census 2022 data, analysing housing pressure and socio-economic inequality across Ireland using K-Means clustering.

Focuses on uncovering hidden territorial patterns beyond traditional urban–rural classifications.

**Fernando Bermudo**  
Software Developer | Java, Kotlin & Python  

📫 contact@granades.dev  
🌐 https://granades.dev  
💻 https://github.com/Granades  

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook


# 🏠 Housing and Social Inequality in Ireland  
### Territorial Patterns using K-Means Clustering

This project explores **housing pressure and socio-economic inequality across Ireland** using **unsupervised machine learning techniques**.

It applies **K-Means clustering** to identify hidden territorial patterns based on census data, revealing insights that go beyond traditional urban–rural classifications.

---

## 📊 Project Overview

This study analyses data from the **Census 2022 Small Area Population Statistics (SAPS)** to uncover:

- Housing pressure patterns
- Socio-economic inequalities
- Spatial differences between regions

Using clustering techniques, the project groups areas with similar characteristics without predefined labels, enabling **data-driven territorial classification**.

> The analysis follows the **CRISP-DM methodology**, focusing on discovery rather than prediction :contentReference[oaicite:0]{index=0}

---

## 🧠 Key Objectives

- Identify **hidden socio-economic patterns** across Ireland  
- Group areas into meaningful clusters based on:
  - Housing conditions  
  - Labour market structure  
  - Education levels  
- Compare results with official **Urban–Rural classifications**  
- Demonstrate the value of **unsupervised learning in real-world analysis**

---

## 🗂️ Dataset

- Source: **Central Statistics Office (CSO) – Ireland**
- Dataset: **SAPS 2022**
- Coverage: ~19,000 small areas (80–120 households each)

The dataset includes socio-economic indicators such as:

- Housing structure (rent, ownership, dwelling type)
- Overcrowding
- Labour market composition
- Education levels

---

## ⚙️ Methodology

### 🔹 CRISP-DM Workflow

1. Business Understanding  
2. Data Understanding  
3. Data Preparation  
4. Modelling  
5. Evaluation  

---

### 🔹 Data Preparation

- Selected **11 key variables**
- Removed missing and invalid values
- Standardised data using **Z-score normalisation**

---

### 🔹 Model

- Algorithm: **K-Means Clustering**
- Distance-based approach → requires standardisation  
- Optimal clusters selected using **Elbow Method**

👉 Final choice: **K = 4 clusters** for better interpretability :contentReference[oaicite:1]{index=1}

---

## 📈 Results

The model identified **4 distinct socio-economic clusters**:

### 🟢 Cluster 0 – Stable & Low Pressure
- Low overcrowding  
- Strong labour market  
- Better living conditions  

### 🟡 Cluster 1 – Transitional Areas
- Moderate housing pressure  
- Mixed socio-economic conditions  
- Often suburban or satellite towns  

### 🔴 Cluster 2 – High Vulnerability
- High social housing  
- Overcrowding  
- Lower education & employment levels  

### 🔵 Cluster 3 – Urban Pressure Zones
- High private renting  
- Dense urban environments  
- Strong economy but high housing stress  

👉 These clusters reveal patterns not fully captured by official classifications :contentReference[oaicite:2]{index=2}

---

## 🔍 Key Insights

- Housing pressure is **not only urban**
- Significant **internal inequality within official categories**
- Transitional areas play a key role in housing dynamics
- Data-driven clustering reveals **hidden socio-economic structures**

---

## 📊 Visualisations

## 📊 Visualisations

### 🔹 1. Exploratory Data Analysis (EDA)

#### Distribution of key variables
![EDA Distribution](images/1_eda_distribution.png)

Initial exploration of the dataset to understand variable distributions and detect skewness or anomalies.

---

#### Overcrowding index by original classification
![EDA Overcrowding](images/2_eda_overcrowding_by_original.png)

Shows how overcrowding varies across traditional classifications (e.g. urban vs rural).

---

### 🔹 2. Choosing the Number of Clusters

#### Elbow Method
![Elbow Method](images/3_elbow_method.png)

Used to determine the optimal number of clusters.  
The curve suggests **K = 4** as a good balance between simplicity and explanatory power.

---

### 🔹 3. K-Means Clustering Results

#### Cluster formation
![K-Means Clusters](images/4_kmeans_clusters.png)

Visual representation of how data points are grouped using K-Means.

---

#### Cluster distribution
![Cluster Distribution](images/5_cluster_distribution.png)

Shows how many areas belong to each cluster.

---

### 🔹 4. Socio-Economic Interpretation

#### Overcrowding by cluster
![Overcrowding by Cluster](images/6_overcrowding_by_cluster.png)

Highlights differences in housing pressure across clusters.

---

#### Original classification vs clusters
![Original vs Clusters](images/7_original_vs_clusters.png)

Comparison between traditional classifications and machine learning clusters.

---

### 🔹 5. Feature Relationships

#### Feature scatter plot
![Feature Scatter](images/8_feature_scatter.png)

Explores relationships between key variables used in clustering.

---

#### Cluster heatmap
![Cluster Heatmap](images/9_heatmap_clusters.png)

Summarises the profile of each cluster across all variables.


---

## ⚠️ Limitations

- K-Means assumes spherical clusters  
- Sensitive to initialisation  
- Results are **descriptive, not predictive**


## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Granades/housing-inequality-ireland-ml.git
cd housing-inequality-ireland-ml
### 2. Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```bash
### 3. Run the notebook
jupyter notebook
