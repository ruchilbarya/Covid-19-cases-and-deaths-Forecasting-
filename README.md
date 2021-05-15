# Covid-19 Cases and Deaths Forecasting
_Time series Analysis_

The objective of this study to predict number of Covid-19 cases and deaths for India and USA respectively and to find out if the number of deaths are related to the Covid-19 cases. Also, I tried to find the relationship between the covid-19 cases in India and USA. Please check out my [Rpubs](https://rpubs.com/Ruchil/770013) for entire code.

## Summary

As per the forecast for the USA covid-19, the cases are like to increase gradually and deaths will also increase with some dropAs per the forecast for the India covid-19, the cases are like to increase exponentially and deaths will also increase but the Indian forecasts were increasing on a steady rate , while USA forecast had lots of ups and downs. Forecasted model for the number of cases had good accuracy and AIC for both India and USA. The relationship between the deaths and cases was not significant for India but it was significant for USA.The relationship between the India and USA cases was not significant. 

The model consists of three main componenets 
* Time series creation with weekly frequency
* Model creation 
* Model evaluation 

## Data 

The dataset for confirmed Covid-19 cases and deaths in USA was obtained from ‘Kaggle’[link](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset) and in India was obtained from ‘Covid19India' dashboard. There are two different datasets for India and USA. The dataset includes Covid-19 cases and deaths from 22 January 2020 to 19 July 2020.

## Methodology 

Four different time series were created for Covid-19 cases in USA ,Covid-19 cases in India, Deaths due to Covid-19 in USA and Deaths due to Covid-19 cases in India with a frequency of 7 (weekly).The start date for all time series was taken as 16th March 2020 and end date was taken as 12th July 2020.The prediction was made for 1 week from 13th July to 19th July 2020. Decomposition was used to detrend the time series and to find if the prediction will increase or decrease based on the time trend.

Cross correlation was used to identify the relation between India and USA covid-19 cases. ADF test was used to check the non-stationary series. Differencing was used to make the series stationary. All time series were converted to a stationary time series before application of any model. AIC was used to find the best model. Mean Absolute percentage error was used to test the accuracy.

## Results

![image](https://user-images.githubusercontent.com/70984576/118362772-f2cce680-b55e-11eb-9d16-3e25fa3fce28.png)

