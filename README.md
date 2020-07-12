# stockprediction
Uses machine leaning to train models that predict profitable stocks 
FINANCIAL STOCK INDICATORS

Datasets
(a) [train] Stock_train.csv
(b) [test] Stock_test.csv]
The TRAIN dataset contains more than 200 financial indicators on almost 5000
stocks. The financial indicators are related to the 2017 and they are used to predict if the stock price of the companies in the dataset have increased in 2018. If the
stock has increased during the 2018, then its class value will be equal to 1, otherwise,
if the stock price has decreased the class value will be equal to 0.
The TEST dataset contains the same 200+ financial indicators on almost 5000 stocks.
The financial indicators are related to the 2018 and they are used to predict if the
stock price of the companies in the dataset have increased during 2019. 

We use Pandas, NumPy, SciKit Learn, Tensorflow, Keras, MatPlotLib libaries on python. 

We the Stock_train.csv dataset to train algorithms with Cross Validation, select the best one with the hypeparameters properly calibrated and then apply the model to the Stock_test.csv in order to predict the class for all the stocks.

We used 6 different classification algorithms to train our model - 
  - Lasso Classification with Penalization
  - Ridge Classification with Penalization
  - Random Forest Classification 
  - Random Forest Classification with ADA boosting
  - Random Forest Classification with Gradient Boosting
  - Neural Networks
  
After training, we evaluate the portfolio performance by doing the following:
Using the Yahoo finance API, we download the price for the stocks the model deems profitable, for the last day of 2018 and the last day of 2019.
Compute the change in the price for each of the selected stock as Price_2019 – Price_2018.
Supposing we have bought one quantity of each of the selected stock, we compute the absolute variation of the value of our portfolio.
