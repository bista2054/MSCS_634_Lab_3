# MSCS_634_Lab_3 - Clustering Analysis Using K-Means and K-Medoids Algorithms

## Purpose

This lab explores unsupervised clustering techniques using the Wine dataset from the sklearn library. The objective is to apply and compare two clustering algorithms, K-Means and K-Medoids, to understand their effectiveness in grouping data points based on chemical properties of wines. The lab also demonstrates how to evaluate clustering quality using metrics like Silhouette Score and Adjusted Rand Index (ARI).

## Key Insights and Observations

- Both K-Means and K-Medoids were able to identify clusters corresponding to the three wine classes.
- K-Means achieved slightly higher Silhouette Score and ARI, indicating more well-defined and accurate clusters on this dataset.
- Visualizations showed that K-Means clusters tend to be more spherical, while K-Medoids handled cluster shapes and potential outliers differently by selecting actual data points as centers.
- K-Medoids may be preferable for datasets with noise or outliers, though it is generally slower compared to K-Means.
- The choice between algorithms depends on the dataset characteristics and the importance of robustness to outliers.

## Challenges and Decisions

- Installing and using the `scikit-learn-extra` library was necessary to access the K-Medoids algorithm but not compatible with recent version so I had to degrade the numpy version.
- Standardizing the dataset via z-score normalization was critical to ensure fair clustering as features have different scales.
- Dimensionality reduction with PCA was employed to visualize high-dimensional clustering results effectively.
- Deciding on cluster count was straightforward since the Wine dataset has three known classes.

---

