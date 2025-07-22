# 🛍️ Mall Customer Segmentation

This project performs **customer segmentation** using various clustering algorithms on the Mall Customers dataset. The goal is to identify distinct groups of customers based on their demographics and spending behavior to enable personalized marketing strategies.

---

## 📊 Dataset

**Source:** [Mall_Customers.csv](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial)

**Features:**
- `CustomerID`: Unique identifier
- `Genre`: Gender (Male/Female)
- `Age`: Customer's age
- `Annual Income`: (k$)
- `Spending Score`: Assigned by the mall based on customer behavior

---

## 🧪 Project Workflow

### 1. **Data Preprocessing**
- Checked for nulls
- Encoded `Genre` using one-hot encoding
- Dropped `CustomerID`
- Scaled features using `MinMaxScaler`

### 2. **Clustering Techniques**
- **KMeans Clustering** (with Elbow Method)
- **Agglomerative Clustering** (Ward linkage + Silhouette Score)
- **MeanShift Clustering**
- **Gaussian Mixture Models (GMM)**
- **DBSCAN** (with tuning via K-distance plot)

### 3. **Evaluation**
- Silhouette Score
- Number of clusters
- Visual comparison of clustering outputs

---

## 📈 Visualizations

- Elbow plot to find optimal `k` for KMeans
- Silhouette scores for Agglomerative clustering
- Cluster scatter plots (2D) for each method
- K-distance graph for DBSCAN tuning

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 📎 Sample Results

| Algorithm         | No. of Clusters | Evaluation Method       |
|------------------|------------------|--------------------------|
| KMeans            | 5                | Inertia (Elbow Method)  |
| Agglomerative     | 4-5              | Silhouette Score        |
| MeanShift         | ~3               | Auto-detected           |
| GMM               | 5                | Probabilistic Clustering|
| DBSCAN            | Varies           | Density-based            |

---

## 📌 Conclusion

KMeans and GMM provided the most balanced clusters. DBSCAN and MeanShift were useful for density-based and automatic clustering but needed careful tuning. These clusters can be used for **targeted marketing** and **customer insights**.

---

## 🚀 Future Improvements

- Integrate PCA/TSNE for better visualization
- Add cluster profiling reports
- Deploy using Streamlit for interactive analysis

---

## 🔗 Author

**Guru Prasath**  
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/guruprasath-nareshkumar-92a976211/) or check out my other projects!

