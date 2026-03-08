# Covid19-Forecasting-ARIMA-JohnsHopkins
Time Series Forecasting of COVID-19 cases using ARIMA and Autoregressive models with Johns Hopkins dataset.
COVID-19 Forecasting using ARIMA
Johns Hopkins Global COVID-19 Dataset
## Project Overview

* This project analyzes global COVID-19 data and predicts future confirmed cases.

* The dataset is obtained from the COVID-19 data repository of Johns Hopkins University.

* Time-series forecasting techniques such as ARIMA and Autoregressive (AR) models are used.

* The objective is to understand pandemic trends and forecast future case growth.

* The project helps demonstrate how data science can support public health planning and decision-making.

## Business Problem

* Governments faced difficulty predicting the rapid spread of COVID-19.

* Without accurate forecasts, it was challenging to:

* Plan hospital beds and ICU facilities.

* Manage oxygen and medical supplies.

* Deploy healthcare staff efficiently.

* Take early preventive measures.

This project provides data-driven forecasts to support better healthcare planning.

## Domain

**Domain: Healthcare Analytics**

**Problem Type: Time Series Forecasting (Regression)**

## Dataset

**Dataset Source: Johns Hopkins Global COVID-19 Dataset**

Files used:

* time_series_covid19_confirmed_global.csv

* time_series_covid19_deaths_global.csv

* time_series_covid19_recovered_global.csv

### Dataset contains:

* Province/State

* Country/Region

* Latitude and Longitude

* Daily cumulative confirmed cases

* Daily cumulative deaths

* Daily recovered cases

## Technologies Used

* Python

* Pandas

* NumPy

* Matplotlib

* Seaborn

* Scikit-learn

* Statsmodels

## Project Workflow
 **Data Collection**

* Collected global COVID-19 time series dataset.

**Data Preprocessing**

* Aggregated data at country level (India).

* Converted dataset into time-series format.

* Created daily confirmed and death cases.

**Exploratory Data Analysis**

* Trend visualization of confirmed and death cases.

* Daily case growth analysis.

* Rolling mean and rolling standard deviation analysis.

* Correlation analysis between confirmed and death cases.

**Time Series Analysis**

* Stationarity testing using ADF test.

* Autocorrelation analysis using ACF plots.

* Differencing applied to make data stationary.

## Key Insights from Analysis

* Confirmed COVID-19 cases show exponential growth trend.

* Death cases increase as confirmed cases increase.

* Strong positive correlation between confirmed cases and deaths.

* Pandemic data shows high variability during peak periods.

**Correlation value:**

0.99

* This indicates a very strong positive relationship.

##  Forecasting Models Implemented
**ARIMA Model**

* Used for time-series forecasting.

* Initial parameters: (1,1,1)

* Autoregressive (AR) Model

* Predicts values based on past observations.

* Initial lag value: 7

## Hyperparameter Tuning

* Grid search used to identify optimal ARIMA parameters.

* Best ARIMA configuration:

ARIMA (3,1,5)

* Best AR lag value:

Lag = 14

## Model Evaluation Metrics

* Models evaluated using:

1)Mean Absolute Error (MAE)

2)Root Mean Squared Error (RMSE)

3)Model	Parameters	MAE	RMSE
ARIMA (Initial)	(1,1,1)	163,922	218,835
AR (Initial)	lag=7	292,108	408,785
ARIMA (Tuned)	(3,1,5)	122,112	170,743
AR (Tuned)	lag=14	17,699	22,221

 **Best Model**

### ARIMA (3,1,5)

**Reasons:**

* Captures long-term growth patterns.

* Handles exponential trends effectively.

* Provides reliable forecasting for pandemic planning.

## Business Impact

* This project helps:

* Forecast COVID-19 case growth.

* Plan hospital and ICU capacity.

*  oxygen and medical supplies.

* Prepare healthcare systems in advance.

*Support data-driven government decisions.

## Challenges Faced

* Missing values in Province/State column.

* Non-stationary time series data.

* Selecting optimal ARIMA parameters.

* Forecast errors during sudden case spikes.

### Solutions used:

* Country-level aggregation.

* Differencing and ADF test.

* Grid search with AIC.

* Model comparison using MAE and RMSE.

## Future Improvements

* Implement LSTM deep learning forecasting model.

* Add Prophet time-series model.

* Forecast cases for multiple countries.

* Create interactive dashboard for visualization.

* Deploy model using Streamlit.

## Conclusion

* Time-series forecasting techniques like ARIMA can effectively predict pandemic trends.

* Data-driven forecasting can help governments plan healthcare resources.

* This project demonstrates the application of data science in healthcare analytics.


Prachi Patel
Aspiring Data Scientist | Machine Learning Enthusiast
