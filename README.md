# M18-Cryptocurrencies

## Overview

This project is about unsupervised machine learning data analysis. First, we have to process data, cluster, reduce dimensions, and reduce the principal components using PCA.

The data will be working with is about Crypto Currencies, so it will need to be processed to fit the machine learning models. Since there is no known output that we are looking for, we have decided to use unsupervised learning. To group the cryptocurrencies, we have decided on a clustering algorithm. We used data visualizations to share the findings with the board.

## Results 

### Preprocessing the Data for PCA

- Read in the data crypto_data.csv to the Pandas DataFrame named crypto_df
- Transform the dataframe to fit the model 
- Create a new DataFrame to store all cryptocurrency names from the CoinName 
- The get_dummies() method is used to create variables for the text features, which are then stored in a new DataFrame
- The features from the X DataFrame have been standardized using the StandardScaler fit_transform() function


<img width="790" alt="DF" src="https://user-images.githubusercontent.com/91625564/154880617-4b33b806-5277-45cd-9e9d-a8d8bc77e171.png">


### Reducing Data Dimensions Using PCA

- Apply PCA to reduce the dimensions to three principal components

### Clustering Cryptocurrencies Using K-means

- Create an elbow curve using hvPlot to find the best value for K from the pcs_df

<img width="790" alt="elbow_plot" src="https://user-images.githubusercontent.com/91625564/154880774-27fe4abd-72d7-47f0-af3e-00fbb6b95bac.png">


### Visualizing Cryptocurrencies Results

- Used knowledge of creating scatter plots with Plotly Express and hvplot, we visualized the distinct groups that correspond to the three principal components we created, then we created a table with all the currently tradable cryptocurrencies using the hvplot.table() functio
- 3D scatter plot using the Plotly Express 

<img width="790" alt="3D_plot" src="https://user-images.githubusercontent.com/91625564/154880726-55ec2e82-79aa-411e-ae3b-14126f490f03.png">

- A hvplot scatter plot is created where the X-axis is "TotalCoinsMined", the Y-axis is "TotalCoinSupply", the data is ordered by "Class", and it shows the CoinName when you hover over the data point 

<img width="790" alt="scatter_plot" src="https://user-images.githubusercontent.com/91625564/154880745-78c85320-e7e5-49e3-ae83-59106bae8cd8.png">


## Summary 

Since there is no known output that we are looking for, we have decided to use unsupervised learning. To group the cryptocurrencies, we have decided on a clustering algorithm. We used data visualizations to share the findings with the board.




