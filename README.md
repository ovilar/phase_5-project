# Time Series Forecasting: NYISO Hourly Load
In this project, I work with data collected from the New York Independent 
System Operator 
(NYISO). The dataset hourly load estimates for all of the New York Zones 
and daily weather data.
I analyze these series using three modeling frameworks and provide 
recommendations for the 
stakeholder.

The modeling framework is streamlined as follows: time series analysis, 
basic and rolling 
statistics, seasonal decomposition, unit-root test, SARIMAX modeling, 
Long Short-Term Meory (LSTM) 
and the use of Facebook's Prophet.

## Business Problem
The stakeholder is the NYISO. A well-function system, which relies on 
accurate 
forecasts, avoid the social and economic costs of grid problems, such as 
blackouts, brownouts, etc. 

Specifically taking a look at the New York City Zone (NYISO J), I provide 
three modeling frameworks 
that aim to reduce forecasting deviations.

## Data and Analysis
The dataset used is a collection of hourly load usage across the NYISO. 
To simplify our analysis, I 
focus only on the NYC Zone (NYISO Zone J). The data spans from 2018 
through 2020. I also provide 
weather statistics and feature engineering.

## Time Series Workflow
I start with testing stationarity and performing a seasonal decomposition 
to assess the best 
combination of Autoregression Integrated Moving Average factors (i.e. p, 
d, q) and Seasonal Factors 
(p, d, q, s). Given computational constraints, I limit those to 1 round 
of runs (even though I also 
provide examples with 2 runs). Then, Autocorrelation and Partial 
Autocorrelation plots are provided 
to check the consistency of the seasonal decomposition findings. Lastly, 
I perform Root-Mean Square 
tests on both training and testing data - which both provide satisfying 
results for our three 
locations.

## Conclusion
Using a time series approach I provide a SARIMAX model that is able to 
perform well both with 
training and testing data. Root-mean squared errors are less than 3% of 
the historical mean prices. 
Thus, one can infer the model is good to predict with a certain accuracy 
house prices. The model is 
inversely as good as the time horizon increases, so for shorter-term 
forecast (up to 24-months) we 
have more precise price estimates. Mean Prices Forecast - 60-month window

### Takeaways and Recommendations

Here you will find:

<ul>
<li>Presentation file;</li>
<li>Jupyter Notebook;</li>
<li>README.md file;</li>
<li>Image Folder;</li>
<li>Data (.CSV) folders.</li>
</ul>
Feel free to reach out if you have any critique, suggestion or 
correction.
# 
Initial README.md file
