# Readme for CSCI 349 Final Project - Nick Satriano, Jake Luther, and Jake Etzler

We are mining historical data from the United States Stock Market to determine how well we can predict the daily trends of stock prices. The stock tickers that we chose to model are PNM, GALT, and AMZN, which represent the following companies in respective order: PNM Resources Inc, Galectin Therapeutics Inc, and Amazon.

The data was obtained through the yfinance python package. Here's a link to the yfinance docs: https://pypi.org/project/yfinance/

Here's a link to our video: https://drive.google.com/file/d/11YjErknpAS4fCJjuME9lxOJAF7eMXBDv/view?usp=share_link

**Full list of packages we used:**  
1) yfinance
2) numpy
3) matplotlib
4) pandas
6) sci-kit learn
7) statsmodels
8) datetime
9) seaborn
10) calendar


**What we found:**  
We found that we had the best results when using a random forest classifier to model our data. With this, we were able to achieve above a 50% precision rate with our model for all three of the stock tickers that we were attempting to predict. To further strengthen our predictions, we created a backtest function which allows us to fit our model iteratively over each year of a decade of data.  

With the current performance metrics that our model is producing, we cannot recommend purely buying and selling stock based off the model's predictions. What we can safely say is that our model has proven itself to be a valid tool in evaluating potential day-to-day trends of a stocks price. One very good use for our model would be if it were used in a suite of metrics for determining stock movement. Our previous work with the Prophet model has proven that it also has validity in determining stock movement, and potentially utilizing these 2 models together could lead to higher precision scores for our predictions.