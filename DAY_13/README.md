# Day 13: Clustering Algorithms

Welcome to **Day 13** of the 30-Day Machine Learning series! In this session, we dive into **Clustering Algorithms**, a fundamental concept in unsupervised learning. This README provides a concise overview, along with code snippets and links to additional resources.

---

## Overview
Clustering involves grouping similar data points together based on their inherent structure. Unlike supervised learning, clustering algorithms work without labeled data, making them ideal for:
- Customer segmentation
- Anomaly detection
- Image compression

### Key Algorithms Covered:
1. **K-Means Clustering**: Efficient for spherical and evenly sized clusters.
2. **DBSCAN**: Ideal for arbitrary-shaped clusters and detecting outliers.
3. **Hierarchical Clustering**: Builds a dendrogram to visualize the clustering process.

---

## Key Concepts

### 1. K-Means Clustering
- Partitions data into `K` clusters by minimizing variance within clusters.
- Requires selecting the optimal `K` (Elbow Method).

#### Code Example:
```python
from sklearn.cluster import KMeans
import matplotlib.pyplot as plt

# Define the model
kmeans = KMeans(n_clusters=3)
kmeans.fit(X)

# Plot the results
plt.scatter(X[:, 0], X[:, 1], c=kmeans.labels_, cmap='viridis')
plt.scatter(kmeans.cluster_centers_[:, 0], kmeans.cluster_centers_[:, 1], s=200, c='red')
plt.show()
```

### 2. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
- Groups points in dense regions, identifies outliers.

#### Code Example:
```python
from sklearn.cluster import DBSCAN

# Define the model
dbscan = DBSCAN(eps=0.5, min_samples=5)
labels = dbscan.fit_predict(X)

# Plot the results
plt.scatter(X[:, 0], X[:, 1], c=labels, cmap='viridis')
plt.show()
```

### 3. Hierarchical Clustering
- Builds a tree-like dendrogram to visualize clustering.

#### Code Example:
```python
from sklearn.cluster import AgglomerativeClustering
import scipy.cluster.hierarchy as sch

# Define the model
hierarchical = AgglomerativeClustering(n_clusters=3)
hierarchical.fit(X)

# Plot dendrogram
dendrogram = sch.dendrogram(sch.linkage(X, method='ward'))
plt.show()
```

---

## Evaluation Metrics

### 1. Silhouette Score
Measures how similar a point is to its cluster compared to other clusters. Ranges from -1 (poor) to 1 (excellent).
```python
from sklearn.metrics import silhouette_score
score = silhouette_score(X, labels)
print("Silhouette Score:", score)
```

### 2. Davies-Bouldin Index
Lower values indicate better clustering.
```python
from sklearn.metrics import davies_bouldin_score
db_index = davies_bouldin_score(X, labels)
print("Davies-Bouldin Index:", db_index)
```

---

## Resources

- **Books**:
  - *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* by Aurélien Géron
  - *Python Machine Learning* by Sebastian Raschka

- **Documentation**:
  - [Scikit-learn Clustering](https://scikit-learn.org/stable/modules/clustering.html)
  - [Scipy Hierarchical Clustering](https://docs.scipy.org/doc/scipy/reference/cluster.hierarchy.html)

- **YouTube Tutorials**:
  - [StatQuest: Clustering](https://www.youtube.com/watch?v=EItlUEPCIzM)
  - [Simplilearn: DBSCAN Clustering](https://www.youtube.com/watch?v=ukC3r7VfTeo)
  - [Corey Schafer: Hierarchical Clustering](https://www.youtube.com/watch?v=ZA9TdCMZLU8)

---

## GitHub Repository
Explore the code for Day 13 and the entire 30-Day Machine Learning series:

🔗 [GitHub Repository: 30DaysML](https://github.com/yourusername/30DaysML)

---

Stay tuned for **Day 14: Dimensionality Reduction**, where we explore techniques like PCA, t-SNE, and UMAP to simplify and visualize high-dimensional data. 🚀
