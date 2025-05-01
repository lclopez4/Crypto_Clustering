Crypto Clustering with K-Means and PCA

This project applies clustering techniques to analyze cryptocurrency performance trends using historical market data. The objective is to segment cryptocurrencies into distinct behavioral groups based on their percentage changes across multiple time frames. This clustering helps identify meaningful patterns in the crypto market and visualize them through dimensionality reduction.

Project Goals

- Normalize and prepare real-world crypto market data
- Apply the K-Means clustering algorithm to identify distinct groups
- Use Principal Component Analysis (PCA) to reduce dimensionality
- Visualize the clustering results in both 2D and interactive formats
- Compare elbow curves from original vs. PCA-reduced datasets

Key Technologies

- Python (Pandas, scikit-learn, Matplotlib, hvPlot)
- Jupyter Notebook
- K-Means Clustering
- Principal Component Analysis (PCA)
- Git / GitHub

Methodology

1. Data Preparation  
   Percentage change data was normalized using `StandardScaler` to ensure fair comparison across coins.

2. Elbow Method  
   The elbow method was used to determine the optimal number of clusters (`k`). Both the original and PCA-reduced datasets suggested `k = 4` as the most stable choice.

3. Dimensionality Reduction with PCA  
   PCA was used to reduce the dataset to three principal components, preserving variance while simplifying visualization and processing.

4. K-Means Clustering  
   The KMeans algorithm was applied to both the original and PCA-reduced data. Cluster labels were then used to group cryptocurrencies based on performance patterns.

5. Visualization  
   Interactive scatter plots (via `hvPlot`) were created to display clusters, with color-coded groups and hover information to explore each cryptocurrency.

Findings
- Optimal Clusters: 4 distinct clusters captured the dominant performance patterns.
- Dimensionality Tradeoff: PCA reduced complexity without significantly impacting cluster quality.
- Visual Insight: Clear, interpretable clusters emerged, offering insight into market behaviors.
