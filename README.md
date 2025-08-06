# 🛍️ Mall Customer Segmentation using K-Means and DBSCAN

This project performs customer segmentation on the **Mall_Customers** dataset using **K-Means** and **DBSCAN** clustering techniques. It includes data preprocessing, cluster visualization, and analysis of customer spending behavior.

---

## 📁 Dataset

**`Mall_Customers.csv`**  
Columns:
- `CustomerID`  
- `Gender`  
- `Age`  
- `Income(k$)`  
- `Spending Score`

---

## 🧱 Project Structure

```
📦 project/
├── model.py                     # Main Python script
├── Mall_Customers.csv           # Dataset
└── README.md                    # This file
```

---

## 🧪 Steps Performed

### 1. 📊 Data Preprocessing
- Removed missing values.  
- Scaled `Income(k$)` and `Spending Score` using `StandardScaler`.

### 2. 📈 K-Means Clustering
- Used **Elbow Method** to choose the optimal number of clusters.
- Trained `KMeans` with `k=5`.
- Plotted customer clusters using unscaled values.
- Plotted **Average Spending Score per Cluster** using bar chart.

### 3. 📉 DBSCAN Clustering
- Optimized `eps` and `min_samples` using **Silhouette Score**.
- Filtered invalid cluster counts (fewer than 2 or more than 50).
- Visualized DBSCAN clusters including **outliers**.
- Plotted **Average Spending Score per DBSCAN Cluster**.

---

## 📌 Key Libraries

- `pandas`  
- `matplotlib.pyplot`  
- `scikit-learn`  
- `numpy`  
- `itertools`

---

## 📊 Output Visuals

- Scatter plots for:
  - Raw customer income vs. spending  
  - K-Means clusters with centroids  
  - DBSCAN clusters with outliers  
- Bar plots of **average spending scores** by cluster (both methods)

---

## 📝 How to Run

1. Make sure you have `Mall_Customers.csv` in the same directory.
2. Install dependencies:

```bash
pip install pandas scikit-learn matplotlib numpy
```

3. Run the script:

```bash
python model.py
```

---
