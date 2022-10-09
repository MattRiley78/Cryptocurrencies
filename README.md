# Cryptocurrencies
## Purpose of Analysis
For Accountability Accounting, an unsupervised Machine Learning model is requested to analyze current cryptocurrency trading data.  The purpose is to sort and create a classification system based on existing data.  Final Data Visualization models are requested to show results.

## Overview of Methods
All Unsupervised Machine Learning methods were employed in a Machine Learning environment in Jupyter Notebook.  The Analysis was broken down into 4 general steps:
1. Preprocessing the Data
2. Reducing Dimensions using PCA (Principal Component Analysis)
3. Clustering Data using K-Means Algorithm
4. Visualizing Results

## Results 
### **1.** PreProcessing
- Only currently traded crypto was kept.
- All cryptocurrencies had a working algorithm.
- "IsTrading" column removed.
- Rows with null values removed.
- Rows with 0 coins (or less?) mined were removed.
- "CoinName" column removed.

- DataFrame modified with GetDummies method.

- Resulting Dataframe Scaled with StandardScaler.

### **2.** Reducing Dimensions using PCA
PCA applied to fit and transform data.  Data loaded into DataFrame with existing indices.

### **3.** Clustering Data using K-Means Algorithm
- Elbow Curve was plotted to find best value for k.

- Using k=4, predictions were created using K-Means algorithm.
- New DataFrame created concatenating all data.

### **4.** Visualizing Results
- 3D Figure created showing PCA data and clusters.

- Table created showing tradable cryptocurrencies.

- TotalCoinSupply and TotalCoinsMined were scaled and loaded into new dataframe in order to create final scatter plot.

- Final Scatter Plot created.


