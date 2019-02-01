# Web-traffic
Time series analysis 

The problem is from Kaggle finished competition.
https://www.kaggle.com/c/web-traffic-time-series-forecasting
In given datasets there are around 150000 time series which represent views of different Wikipedia pages. The main goal of the competition was to predict those series.
The idea to predict all those time series separately is doable, however I will group them and approximate behavior of each page views with the trend of the group as a whole. The idea is to model the mean value among all time series in the group for each day.
The approach to the group division depends on the result you want to achieve. I will explore separation by language, by access to the page and by type of the cite (wikipedia, wikimedia or mediawiki).
The predictions are done with fbProphet and compared to LSTM predictions.
