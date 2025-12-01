# Iris Clustering Analysis (K-Means & Hierarchical Clustering)

## Overview
This project applies two unsupervised machine learning techniques — **K-Means Clustering** and **Agglomerative Hierarchical Clustering** — to the Iris dataset.  
The goal is to explore the natural structure of the data, determine the optimal number of clusters, visualise cluster formation, and interpret the results.

## Objectives
- Load and preprocess the Iris dataset.
- Apply **K-Means clustering** and determine the optimal number of clusters using:
  - Elbow Method
  - Silhouette Score
- Apply **Agglomerative Hierarchical Clustering** with dendrogram visualisation.
- Generate 2D and 3D cluster visualisations.
- Interpret the clustering patterns for both methods.
- Compare K-Means and Hierarchical Clustering.

## Dataset
The Iris dataset consists of:
- 150 flower samples  
- 4 numerical features:  
  - Sepal Length  
  - Sepal Width  
  - Petal Length  
  - Petal Width  
- 3 species (used only for reference; clustering is unsupervised).

## Methodology

### 1. K-Means Clustering
- Used the Elbow Method to determine candidate cluster counts.
- Evaluated **k = 2** and **k = 3** using Silhouette Score.
- Chose **k = 2**, which produced the highest Silhouette Score.
- Generated 2D and 3D visualisations.
- Interpreted cluster assignments based on centroid values.

### 2. Hierarchical Clustering
- Generated a dendrogram using Ward linkage.
- Identified **2 natural clusters** from the largest vertical separation.
- Applied **AgglomerativeClustering (n_clusters = 2)**.
- Plotted 2D and 3D cluster diagrams.
- Interpreted the hierarchical grouping patterns.

### 3. Comparison of Both Methods
Both algorithms consistently identified:
- One distinct cluster corresponding to **Iris Setosa**.
- One combined cluster containing **Versicolor and Virginica**, which overlap significantly.

K-Means provides stronger numerical validation (silhouette score), while Hierarchical Clustering provides a clear structural view via the dendrogram.

## File Contents
- **Notebook**: Full code, visualisations, and interpretations.
- **README.md**: Overview of methodology, approach, and conclusions.

## How to Run
1. Install Python 3.8+ with required libraries:
   ```
   pip install numpy pandas matplotlib scikit-learn scipy
   ```
2. Open the Jupyter notebook:
   ```
   jupyter notebook
   ```
3. Run cells sequentially.

## Conclusion
The Iris dataset naturally forms **two clusters** in feature space.  
Both K-Means and Hierarchical Clustering reveal this structure:
- **Cluster 1**: Setosa (well-separated)
- **Cluster 2**: Versicolor + Virginica (overlapping)

This project demonstrates practical application of unsupervised learning and cluster evaluation techniques.

## License
This project is released for academic and learning purposes.
