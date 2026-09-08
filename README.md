# Assignment 9: Unsupervised Learning

**Name:** OBAJE PAUL
**Course:** MACHINE LEARNING

## Project Overview

This project demonstrates the use of unsupervised learning techniques to identify patterns and groups within the Wine dataset. The analysis focuses on clustering and dimensionality reduction.

## Dataset

The Wine dataset from Scikit-learn was used. It contains **178 observations and 13 numerical features** representing chemical properties of wine samples.

## Preprocessing

The dataset was inspected for missing values and duplicate records. The features were numerical, so one-hot encoding was not required. StandardScaler was used to standardize the features before clustering.

## Clustering Methods

Two clustering techniques were applied:

* K-Means Clustering
* Hierarchical Clustering

The Elbow Method and Silhouette Score were used to determine and evaluate the clustering structure.

## Results

| Method                  | Silhouette Score |
| ----------------------- | ---------------: |
| K-Means                 |           0.2849 |
| Hierarchical Clustering |           0.2774 |

K-Means achieved the higher Silhouette Score and was selected as the better-performing clustering method.

## Dimensionality Reduction

Principal Component Analysis (PCA) was used to reduce the 13 original features to two principal components.

* PC1 explained 36.20% of the variance.
* PC2 explained 19.21% of the variance.
* Together, they explained 55.41% of the total variance.

## Deployment and Monitoring

The K-Means model could be deployed in a wine analysis or segmentation system. New data would need to go through the same preprocessing and scaling process before being assigned to a cluster.

The model can be monitored using cluster sizes, changes in incoming data and Silhouette Scores. If the data distribution changes significantly or clustering quality decreases, the model can be retrained with newer data.

## Files

* `Assignment_9_Unsupervised_Learning_OBAJE_PAUL.ipynb` — Google Colab notebook
* `README.md` — Project documentation

## Tools Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* K-Means
* Hierarchical Clustering
* PCA
