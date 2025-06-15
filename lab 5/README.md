# Lab 5: Clustering Techniques Using DBSCAN and Hierarchical Clustering

## Purpose
In this lab, I applied DBSCAN and Agglomerative Hierarchical Clustering to the Wine dataset. The goal was to explore how these clustering algorithms group the data and how parameter choices affect the results.

## Insights

- Hierarchical clustering produced clear clusters when the number of clusters matched the true wine classes.
- DBSCAN was able to find clusters of varying shapes and identify noise points, but I first had to find the right eps and min_samples values.
- The best DBSCAN results (in terms of silhouette and homogeneity) were achieved with lower min_samples and smaller eps values, but too small values led to many small clusters or excessive noise.

## Challenges

- Finding DBSCAN parameters that produced more than one cluster (excluding noise) required a lot of attempts
