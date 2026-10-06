# Data Mining Techniques

This repository brings together several data-mining methods across association analysis, anomaly detection, dimensionality reduction, web-data extraction and document clustering.

## Association-rule evaluation

Implements the **Kulczynski measure** from frequent-itemset support values by combining confidence in both rule directions.

It also derives the number of possible non-empty itemsets from a collection of N items as **2^N - 1**.

## Outlier detection

The notebook explores several approaches to anomaly detection:

- **IQR-based detection** on monthly rainfall data
- **One-Class SVM** on daily percentage changes for Microsoft, Ford and Bank of America
- **PCA + k-nearest-neighbour scoring** on housing data

In the recorded One-Class SVM run, **127 of 2,517 observations** were classified as outliers, approximately **5.05%** of the dataset.

The housing analysis reduces the original feature space to two principal components before calculating a second-nearest-neighbour distance as an outlier score.

## Web-data extraction

Uses **BeautifulSoup** and pandas to extract, clean and structure tabular HTML data. A local HTML fallback is included for cases where the original endpoint is unavailable.

## Document clustering

Clusters a collection of technical Wikipedia articles using:

- **TF-IDF** text representation
- **K-Means**
- the **elbow method** for choosing the number of clusters

The recorded elbow analysis supports **k = 3** for the final clustering run.

## Tools

**Python · pandas · NumPy · scikit-learn · Matplotlib · BeautifulSoup · TF-IDF · K-Means**

## Notebook

`data_mining_techniques.ipynb`
