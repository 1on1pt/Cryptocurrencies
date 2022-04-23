# Cryptocurrencies
Taking a deeper dive into machine learning by using unsupervised algorithms, for example the K-Means algorithm, to analyze data without a clear output in mind.


## Overview of the Analysis
![popular-cryptocurrencies](https://user-images.githubusercontent.com/94148420/164922829-937b9523-0436-4ce6-ae14-0df3a2794ece.jpeg)

You and Martha have done your research. Data analysis skills in unsupervised machine learning include:
* How to preprocess data - selection, transformation, and scaling
* How to cluster - using elbow curve
* How to reduce dimensions
* How to reduce the principal components using PCA
* How to visualize the results - hvPlot, Plotly

All of these skills are put to use by creating an analysis for clients who are preparing to get into the cryptocurrency market.

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies *are on the trading market* and *how they could be grouped to create a classification system* for this new investment.

The data Martha will be working with is not ideal, so it was processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

### Resources
#### Code:
* crypto_clustering.ipynb

#### Data:
* https://github.com/1on1pt/Cryptocurrencies/blob/main/Resources/crypto_data.csv

#### Software/Data Tools/Libraries:
* Jupyter Notebook 6.4.6
* Python 3.7.11
* scikit-learn
* hvPlot
* StandardScaler
* MinMaxScaler
* PCA
* KMeans

## Results
### Preprocessing the Data for PCA
The original dataset was preprocessed for PCA.  Here is the original dataset as it was loaded into the crypto_df dataframe:
![orig_df](https://user-images.githubusercontent.com/94148420/164934383-722fe87a-8ad8-402b-8395-dedf6653d9da.PNG)

Summary of cleaning/preprocessing the data:
* Keeping all the cryptocurrencies that are being traded
* Keeping all the cryptocurrencies that have a working algorithm
* Removing rows that have at least one null value
* Keeping the rows where coins are mined
* Using get_dummies() to create variables for text features
* Stardarding the data with StandardScaler()

Here is using get_dummies() to create variables for text features:
![get_dummies](https://user-images.githubusercontent.com/94148420/164934926-f668c1d7-1bf8-452b-b0e8-aec6eaad19d3.PNG)

And standardizing the data with StandardScaler():
![stand_scale](https://user-images.githubusercontent.com/94148420/164935244-1d0a13a3-096f-463f-ace9-134c6d3970f1.PNG)


### Reducing Data Dimensions Using PCA
PCA was used to reduce dimension to three principal components:
![pca_reduce](https://user-images.githubusercontent.com/94148420/164935760-59b42fe7-d6ce-4f05-8203-1825bd325222.PNG)

Next, a dataframe was created with the three principal components:
![pcs_df](https://user-images.githubusercontent.com/94148420/164936218-7b7f31cf-d80d-434e-9c25-ae37c88340b7.PNG)



### Clustering Cryptocurrencies Using K-means


### Visualizing Cryptocurrencies Results

## Summary
