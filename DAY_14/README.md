# Day 14: Dimensionality Reduction in Machine Learning  

This repository contains all the code examples, visualizations, and resources for **Day 14** of the **30-Day Machine Learning Learning Path**, focusing on **Dimensionality Reduction** techniques. These techniques are crucial for simplifying high-dimensional data, improving computational efficiency, and enhancing the interpretability of datasets.

---

## **Contents**  

1. **Principal Component Analysis (PCA)**  
   - Explanation of PCA: A linear technique for feature extraction and dimensionality reduction.  
   - Code implementation with Scikit-learn and visualization using the Iris dataset.  
   - Key insights about explained variance and principal components.  

2. **t-Distributed Stochastic Neighbor Embedding (t-SNE)**  
   - Overview of t-SNE: A nonlinear technique for visualizing complex, high-dimensional data.  
   - Implementation with hyperparameter tuning (`perplexity`, `learning_rate`, `max_iter`).  
   - Visualizing clusters and understanding local vs. global structure.  

3. **Uniform Manifold Approximation and Projection (UMAP)**  
   - Introduction to UMAP: Faster and scalable dimensionality reduction.  
   - Implementation with the Iris dataset and parameter explanations (`n_neighbors`, `min_dist`).  
   - Comparison with t-SNE and PCA for preserving structure.  

4. **Comparisons and Key Takeaways**  
   - Side-by-side comparison of PCA, t-SNE, and UMAP.  
   - Best use cases for each technique.  

---

## **Requirements**  

To run the code in this repository, you’ll need the following Python libraries:  

```bash  
pip install numpy pandas scikit-learn seaborn matplotlib umap-learn
```  

---

## **Code Examples**  

The repository includes three separate scripts for each dimensionality reduction technique:  

1. **`pca_example.py`**  
   - Contains PCA implementation with visualization and variance explanation percentages.  

2. **`tsne_example.py`**  
   - Includes t-SNE with tuned hyperparameters for optimal cluster visualization.  

3. **`umap_example.py`**  
   - UMAP implementation with better handling of local and global data structure.  

---

## **How to Run the Scripts**  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/machine-learning-30-days.git  
   cd machine-learning-30-days/dimensionality-reduction  
   ```  

2. Run any script using Python:  
   ```bash  
   python pca_example.py  
   python tsne_example.py  
   python umap_example.py  
   ```  

3. Visualizations will be displayed directly as scatter plots.

---

## **Resources**  

To learn more about the concepts and techniques, refer to these resources:  

- **Principal Component Analysis (PCA)**:  
  - [Scikit-learn PCA Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)  
  - [PCA Explained in 10 Minutes (YouTube)](https://www.youtube.com/watch?v=FgakZw6K1QQ)  

- **t-SNE**:  
  - [Scikit-learn t-SNE Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html)  
  - [t-SNE Visualization and Concepts (YouTube)](https://www.youtube.com/watch?v=NEaUSP4YerM)  

- **UMAP**:  
  - [UMAP Official Documentation](https://umap-learn.readthedocs.io/en/latest/)  
  - [Introduction to UMAP for Dimensionality Reduction (YouTube)](https://www.youtube.com/watch?v=GdRY7xmmswU)  

- **Comparison of Methods**:  
  - [PCA vs t-SNE vs UMAP: Choosing the Right Technique (YouTube)](https://www.youtube.com/watch?v=nZAMzV0G9uY)  

---

## **Key Takeaways**  

- PCA is a linear method, best suited for feature extraction.  
- t-SNE excels in visualizing clusters but can be computationally expensive.  
- UMAP is faster and scalable, preserving both local and global data structures effectively.  
- Choose the technique based on the dataset and task requirements.  

---

## **Author**  

Blog and code written by **Kartik**, as part of the **30-Day Machine Learning Learning Path**.  

For more insights and learning materials, visit the [blog post here](https://medium.com/@gargkartik74/day-14-dimensionality-reduction-d2e4770e4e10).  

---

## **License**  

This repository is licensed under the MIT License.  

--- 

Would you like me to adapt or customize this further?
