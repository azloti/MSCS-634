# Lab 3: Clustering with K-Means and K-Medoids

## Purpose
In this lab, I compared K-Means and K-Medoids clustering on the Wine dataset. The goal was to see how each algorithm groups the data and how well the clusters match the real wine types.

## Insights

- K-Medoids made more natural and clear clusters because it uses real data points as centers.
- K-Means was faster, but its centroids sometimes ended up in empty areas.
- K-Medoids had better scores for both silhouette and ARI, showing it matched the real classes more closely.

## Challenges

- I could not use `scikit-learn-extra` for K-Medoids because of Mac/Apple Silicon issues (some missing headers made it unable to install), so I ended up using `pyclustering` instead. Documentation for that was harder to find than for scikit.
