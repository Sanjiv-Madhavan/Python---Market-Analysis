# Python
I will be uploading all the python projects that I do
These include mainly stock market analysis and value investing analysis
Value analysis is formatted to work with the https://www.equitymaster.com/ website where you can find the statements of Indian companies.
Stock analysis is formatted for information available in https://in.finance.yahoo.com/

# Update (7/26/2020) :

## Machine Learning For Nifty50

I have used **KNN** and **VotingClassifier** to classify the stocks into three categories

1. Buy labelled 1
2. Sell labelled -1
3. Hold labelled 0

The features are the **percentage changes** of the adjusted close values over a period of 7 days. I have made decisions based on **(+/-) 2%** change and assigned labels for the Stocks.

> (Note - I have mentioned all the Stocks by their ticker values as per Nifty.)

Then **pct_change** is used to make the feature set and this is fed into KNN and Voting Classifier that includes KNN, RandomForest and SVM combined. 
Accuracies of the Classifiers are compared.

### Further Readings

- I have gathered the company list from [Wiki for Nifty](https://en.wikipedia.org/wiki/NIFTY_50)
  
  - **BeautifulSoup** is used to scrape this website to get the list of all tickers
  - The yahoo finance website is used to get the dataset of the stocks of these tickers using **Pandas_datareader**

- The dataset is stored inside the `nifty_csvs` folder

- The `main_csv_tickers_joined.csv` contains the Ticker name and the adjusted close values

 
