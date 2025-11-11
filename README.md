Customer Segmentation — Unsupervised Learning on Retail Data
Overview
This project applies unsupervised learning to segment customers using retail transaction data.
Dataset
⦁	Source: UCI Machine Learning Repository – Online Retail Dataset
⦁	Data: Transactions from a UK-based retailer (2010–2011)
⦁	Features: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
⦁	License: See UCI dataset page
Goal
Understand customer purchasing behavior and group customers with similar buying patterns.
Steps
Step 1 — Data Collection
⦁	Downloaded dataset from UCI Repository.
⦁	Loaded using pandas.
⦁	Checked structure, data types, and missing values.
Step 2 — Define the Problem
⦁	Objective: Segment customers using unsupervised learning.
⦁	Business relevance: Supports targeted marketing and personalized strategies.
Step 3 — Exploratory Data Analysis (EDA)
⦁	Inspected data, missing values, and unique customers.
⦁	Cleaned data: removed missing CustomerID rows.
⦁	Created TotalPrice = Quantity × UnitPrice.
⦁	Generated RFM (Recency, Frequency, Monetary) features per customer.
Step 4 — Data Transformation
⦁	Applied log transform to reduce right skewness.
⦁	Used StandardScaler and MinMaxScaler for normalization.
Step 5 — Dimensionality Reduction
⦁	Applied PCA, Truncated SVD, and NMF to explore data structure.
⦁	Visualized explained variance and component distributions.
Step 6 — Clustering
⦁	Performed KMeans clustering.
⦁	Used Elbow method and Silhouette score to find best number of clusters.
⦁	Best silhouette score selected 2 clusters.
⦁	Assigned cluster labels to customers.
Step 7 — Cluster Insights
⦁	Analyzed average RFM values per cluster.
⦁	Interpreted each cluster (e.g., Recency-heavy, Frequency-heavy, Monetary-heavy).
⦁	Visualized distributions with plots.
Step 8 — Summary and Conclusions
⦁	Two main customer segments were found.
⦁	Log transformation and scaling improved performance.
⦁	PCA and NMF helped visualize structure.
⦁	RFM features provided useful insight into customer behavior.
Technologies
⦁	Python, Pandas, NumPy
⦁	Scikit-learn
⦁	Matplotlib
Author
Oliver Vogelgesang  
Course: CSCA 5632 — Unsupervised Learning Final Project
