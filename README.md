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
accurate forecasts with the aim of avoiding the social and economic costs through a fine-tuned operation. 

Specifically taking a look at the New York City Zone (NYISO J), I provide 
three modeling frameworks that aim to reduce forecasting deviations.

## Data and Analysis
The dataset used is a collection of hourly load usage across the NYISO. To simplify our analysis, I 
focus only on the NYC Zone (NYISO Zone J). The data spans from 2018 through 2020. I also provide 
weather statistics and feature engineering.

## Time Series Workflow

### SARIMAX
I start with testing stationarity and performing a seasonal decomposition to assess the best combination of Autoregression Integrated Moving Average factors (i.e. p, 
d, q) and Seasonal Factors (p, d, q, s). Given computational constraints, I limit those to 1 round of runs. Then, Autocorrelation and Partial 
Autocorrelation plots are provided to check the consistency of the seasonal decomposition findings. Lastly, 
I perform a prediction on testing data. Generally, the SARIMAX model is too intensive to be run which limits tuning 
alternatives.

### LSTM
Next, I provide two Long Short-Term Memory Neural Network models. Both the simple and the more structure models provide good 
Mean Absolute Percent Errors and allow for hyperparameter tuning. However, while achieving interesting results, the models 
fail to capture the troughs in the data.

### The Prophet
Lastly, I run two Prophet settings: a plain vanilla one and another with exogenous features. Even though the general load 
pattern resembles the overall data look, the model fails to capture the data peaks. However, it captures the seasonality 
aspects from the data accurately and it might be a good alternative for trough modeling.


## Conclusion
Using a time series approach I provide three hourly load forecasting alternatives: the SARIMAX, the LSTM and the Prophet. 
With the aim of fine tuning grid forecasting the conclusion are as follows.

### Takeaways and Recommendations
The stakeholder could follow three strategies:
<ul>
<li>Using the LSTM to capture data peaks;</li>
<li>Using the Prophet to capture the general shape and data troughs;</li>
<li><b>Ensemble:</b> generating a model tha combines both alternatives listed above for the best load pattern matching 
and reduced MAPEs.</li>
</ul>

### Limitations
The addition of granular data or generation/transmission and weather estimates most likely would improve the results. 
Furthermore computational limitations also impede further and a thorough assessment of hyperparameter tuning.

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
