# Yes Bank Stock Price Prediction 

**Overview**

This project uses machine learning algorithms to predict the stock price of Yes Bank, a leading Indian financial services company. The project utilizes historical stock prices and several features such as Opening, Closing, Highest, lowestprice of the stock  to make the predictions. The machine learning algorithms used include linear regression, Ridge, Lasso, Elastic Net, Random Forest, and Decision Tree.

**Problem Statement**

The problem at hand is to predict the closing price of Yes Bank stock using historical data. The dataset consists of daily stock prices for Yes Bank from May 2005 to September 2020. The aim is to build a regression model that takes into account the opening, high and low prices of the stock as input features and outputs the predicted closing price for the next day.

The model will be trained on the historical data and will be evaluated on a test set of data. The performance of the model will be measured using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), R-squared (R2) score, and Mean Absolute Scaled Error (MASE).

**The main objective is to build an accurate and reliable model that can be used to make predictions about the future closing price of Yes Bank stock. Such a model would be of great value to investors and traders who are looking to make informed decisions about buying, selling, or holding Yes Bank stock.**

**Data**

The dataset used in this project contains monthly stock prices of Yes Bank from 2010 to 2021, along with several features such as company financials (e.g. revenue, net income), economic indicators (e.g. GDP growth, inflation), and news sentiment (e.g. positive/negative news articles). The dataset consists of 133 monthly observations, with each observation containing the following variables:

1. Date: The date (Month and Year provided).

2. Open: The price of the stock at the beginning of a particular time period.

3. High: The peak (maximum) price at which a stock traded during the period.
4. Low: The lowest price at which a stock traded during the period.

5. Close: The trading price at the end (in this case end of the month).

The data was collected from public sources and preprocessed for use in the machine learning models. The dataset was split into training and test sets with a ratio of 80:20, where 80% of the data was used for training the models and 20% for testing.

The dataset contains 185 entries, 0 to 184 with 5 columns each observation containing the stock price and the corresponding values of the features. The dataset was split into training and test sets with a ratio of 80:20, where 80% of the data was used for training the models and 20% for testing.

The data was analyzed using various EDA techniques such as time series plots, histograms, and scatterplots to gain a better understanding of the data characteristics. The data was found to have some trends and seasonality, which were taken into account while building the machine learning models.

**Methodology**

The project used a supervised learning approach to predict the stock price of Yes Bank. First, the data was split into training and test sets. The training set was used to train the machine learning algorithms, and the test set was used to evaluate their performance.

The following machine learning algorithms were used in this project:

* Linear Regression
* Ridge Regression
* Lasso Regression
* Elastic Net Regression
* Random Forest Regression
* Decision Tree Regression
The performance of each algorithm was evaluated using several metrics such as mean squared error (MSE), Root  mean squared error(RMSE), and R-squared (R2) value.

**Results**


The Random Forest algorithm performed the best with a mean squared error of 2.84 and an R-squared value of 0.96. The Linear Regression algorithm also performed well with an R-squared value of 0.92.

**Conclusion**

In conclusion, this project demonstrated the effectiveness of machine learning algorithms in predicting the stock price of Yes Bank. The Random Forest algorithm was found to be the best performing algorithm, followed by Linear Regression. These results can be used by investors and traders to make informed decisions regarding Yes Bank stocks. However, it is important to note that stock prices are influenced by several factors, and the predictions made by these models should be taken as one of several factors to consider when making investment decisions.

After analyzing the Yes Bank stock price data, we can draw the following conclusions:

* Yes Bank's stock price experienced significant fluctuations between 2005 to 2020, indicating a volatile market.

* The monthly moving average analysis suggests that the stock price was declining consistently over time.

* The correlation analysis shows that there is a strong positive correlation between the Open, High, Low, and Close variables, indicating that they all move in the same direction.

* The data is positively skewed and has outliers, indicating that some data points are very different from the others. This indicates that the data might not be normally distributed and needs to be treated before fitting the model.

* The regression analysis shows that the model can predict the closing price of the stock with a reasonable degree of accuracy. However, the model can be improved by tuning the hyperparameters and using different algorithms.


* Overall, the project provides insights into the stock price behavior of Yes Bank, which can be useful for investors and traders in making informed decisions. The project also highlights the importance of data analysis and modeling in understanding the financial market and predicting future trends.


* Using data visualization on our target variable, we can clearly see the impact of 2018 fraud case involving Rana Kapoor as the stock prices decline dramatically during that period.

* After loading the dataset, we found that there are no null values in our dataset nor any duplicate data.
* 
* There are some outliers in our features however this being a very small dataset, dropping those instances will lead to loss of information.
* 
* We found that the distribution of all our variables is positively skewed. so we performed log transformation on them.
* 
* There is a high correlation between the dependent and independent variables. *  This is a signal that our dependent variable is highly dependent on our features and can be predicted accurately from them.
* 
* We found that there is a rather high correlation between our independent variables. This multicollinearity is however unavoidable here as the dataset is very small.
* 
* We implemented several models on our dataset in order to be able to predict the closing price and found that all our models are performing remarkably well

* All of the implemented models performed quite well on our data giving us the Adjusted R-square of over 99%.

* We checked for presence of Heterodasceticity in our dataset by plotting the residuals against the Elastic Net model predicted value and found that there is no Heterodasceticity present. Our model is performing well on all data-points.

With our model making predictions with such high accuracy, we can confidently deploy this model for further predictive tasks using future data.

**Future Scope**

* Based on the analysis performed, there are a few areas that could be explored further:

* Time series modeling: The current analysis focused on descriptive statistics and regression modeling to predict the closing price. However, there is scope to explore time series modeling techniques such as ARIMA or Prophet to better capture the temporal dependencies and trends in the data.

* Feature engineering: The current analysis used only the Open, High, and Low prices as features for the regression model. However, there may be additional features that could be engineered from the data such as trading volumes, news sentiment, or macroeconomic indicators that could improve the model's predictive power.

* Ensemble methods: Another area of exploration could be to use ensemble methods such as random forests or gradient boosting to combine the predictions of multiple models and potentially improve the overall performance.

* External data sources: Finally, incorporating external data sources such as social media sentiment or news articles related to Yes Bank or the banking industry could provide additional insights and potentially improve the model's performance.

