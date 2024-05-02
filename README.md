# Crypto Clustering #
* unsupervised learning challenge

## Instructions ##
1. Prepare the Data
2. Find the Best Value for k Using the Original Scaled DataFrame
3. Cluster Cryptocurrencies with K-means Using the Original Scaled Data
4. Optimize Clusters with Principal Component Analysis
5. Find the Best Value for k Using the PCA Data
6. Cluster Cryptocurrencies with K-means Using the PCA Data

## Sources ##
* 01: standardizing_stock_data
    * to set index
        * df_market_data_scaled.set_index('coin_id', inplace=True)

* 02: [stackoverflow link](https://stackoverflow.com/questions/32857029/python-scikit-learn-pca-explained-variance-ratio-cutoff)
    * find total explained variance
        * np.sum(pca.explained_variance_ratio_)

* 03: [plotly link 3d scatter plot](https://plotly.com/python/3d-scatter-plots/)
    * create 3D scatter plot
        * fig = px.scatter_3d(market_pca_predictions_df, x='PCA1', y='PCA2', z='PCA3', color='pca prediction' , hover_col=['coin_id'])

* 04: [plotly link hover text](https://plotly.com/python/hover-text-and-formatting/)
    * create hover columns in plotly 3D graph
        * hover_data=['coin_id']