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

![D1 1 Crypto_DF](https://user-images.githubusercontent.com/106561880/194784134-b905c7e1-daf1-4b8b-b111-ee199ac87591.png)

- DataFrame modified with GetDummies method.

![D1 2 GetDummies](https://user-images.githubusercontent.com/106561880/194784147-16a39569-2fff-4f72-b8dd-847a621bf7e0.png)

- Resulting Dataframe Scaled with StandardScaler.


### **2.** Reducing Dimensions using PCA
PCA applied to fit and transform data.  Data loaded into DataFrame with existing indices.

![D2 1 PCA](https://user-images.githubusercontent.com/106561880/194784156-c9cdf8c1-acc0-4536-ac0e-99bcdd7e118b.png)


### **3.** Clustering Data using K-Means Algorithm
- Elbow Curve was plotted to find best value for k.

![D3 1 ElbowCurve](https://user-images.githubusercontent.com/106561880/194784164-f014dc65-1cb1-4fa5-aefb-b2d43e7a8793.png)

- Using k=4, predictions were created using K-Means algorithm.
- New DataFrame created concatenating all data.

![D3 2 ClusteredDF](https://user-images.githubusercontent.com/106561880/194784172-3dfb0f78-303a-4247-b33d-4da15afba906.png)

### **4.** Visualizing Results
- 3D Figure created showing PCA data and clusters.

![D4 1 3DPlot](https://user-images.githubusercontent.com/106561880/194784175-171e3cd6-779a-4d3d-8d4b-4c42ea1467fc.png)

- Table created showing tradable cryptocurrencies.

![D4 2 Table](https://user-images.githubusercontent.com/106561880/194784181-2c50831a-b93d-4a5e-ad45-739659e46276.png)

- TotalCoinSupply and TotalCoinsMined were scaled and loaded into new dataframe in order to create final scatter plot.

![D4 3 ScaledDF](https://user-images.githubusercontent.com/106561880/194784189-30971839-5953-4375-82c0-3c0b7ac8c80e.png)

- Final Scatter Plot created.

![D4 4 ScatterPlot](https://user-images.githubusercontent.com/106561880/194784193-c271a72f-22dc-4dfa-ad6d-867be7bd1253.png)


