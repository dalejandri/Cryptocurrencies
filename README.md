# Cryptocurrencies

## Background

<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Cryptocurrencies/blob/main/Resources/1.PNG" /></p>

You and Martha have done your research. You understand what unsupervised learning is used for, how to process data, how to cluster, how to reduce your dimensions, and how to reduce the principal components using PCA. It’s time to put all these skills to use by creating an analysis for your clients who are preparing to get into the cryptocurrency market.

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of your most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.


## Deliverable 1: Preprocessing the Data for PCA 
The following five preprocessing steps have been performed on the crypto_df DataFrame:

- All cryptocurrencies that are not being traded are removed.
- The IsTrading column is dropped.
- All the rows that have at least one null value are removed.
- All the rows that do not have coins being mined are removed.
- The CoinName column is dropped.
- A new DataFrame is created that stores all cryptocurrency names from the CoinName column and retains the index from the crypto_df DataFrame.
- The get_dummies() method is used to create variables for the text features, which are then stored in a new DataFrame, X.
- The features from the X DataFrame have been standardized using the StandardScaler fit_transform() function.

<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Cryptocurrencies/blob/main/Resources/2.PNG" /></p>


## Deliverable 2: Reducing Data Dimensions Using PCA
Apply the Principal Component Analysis (PCA) algorithm, you’ll reduce the dimensions of the X DataFrame to three principal components and place these dimensions in a new DataFrame.

- The PCA algorithm reduces the dimensions of the X DataFrame down to three principal components.
- The pcs_df DataFrame is created and has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df DataFrame.

<p align="center"><img class="centerImage" src="https://github.com/dalejandri/Cryptocurrencies/blob/main/Resources/3.PNG" /></p>
