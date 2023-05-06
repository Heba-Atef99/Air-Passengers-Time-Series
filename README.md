# Airline Passengers Time Series Data Analysis

This a time series data project that applies all the concepts learnt in Time Series Analysis and Forecasting

<p align="center">
  <a href="#dataset">Dataset</a> •
  <a href="#dependencies">Dependencies</a> •
  <a href="#evaluation">Evaluation & Splitting</a> •
  <a href="#forecasting">Forecasting Methodologies</a> •
  <a href="#comparison">Comparison Table</a> •
  <a href="#contributors">Contributors</a>
</p>

## Dataset
[Air Passengers Dataset](https://www.kaggle.com/datasets/abhishekmamidi/air-passengers) contains Number of Air passengers of each month from the year 1949 to 1960. We can use this data to forecast the future values and help the business.

![image](https://user-images.githubusercontent.com/54477107/230594840-46483a93-dafc-491c-b48d-0f452c33daa8.png)

## Dependencies
    Python 3.8.10
    Pandas
    NumPy
    statsmodels
    sklearn
    fbprophet
    xgboost

## Evaluation
### Evaluation Metric
We chose RMSE as our evaluation metric
an absolute error measure that squares the deviations to keep the positive and negative deviations from canceling one another out.

![image](https://user-images.githubusercontent.com/54477107/230594578-6fa8ab4f-a28e-4d19-aeeb-69abb3f65fc5.png)

### Data Splitting
#### Fixed Train Test Split
![image](https://user-images.githubusercontent.com/54477107/230593907-09967430-b951-4e4e-b5e6-a4ef632198e7.png)

#### k-folds Cross Validation
![image](https://user-images.githubusercontent.com/54477107/230593496-f0e40963-2098-4654-870a-b25407eaf890.png)

#### Roll Forward
![image](https://user-images.githubusercontent.com/54477107/230594367-03244202-1832-46a3-9160-c8283afddcb6.png)

## Forecasting
### 1. Simple Moving Average Smoothing

![Alt text](./Simple%20Moving%20Average%20Smoothing.png)

<b>We tried different window sizes, and we noticed that:</b>
* The larger the window size, the more data we <b>lose</b> from the beginning and the end of our timeseries data
* The window size determines the smoothness of the trend-cycle estimate.
* MA technique uses the past series values to forecast. 
</br>

<b>MA disadvantages are:</b>
* Each historical value is given the same weight.
* It's hard to determine the window size (no. of periods used).
* Moreover, each n periods must be stored in the system.
---

### 2. Naïve Forecasting

![Alt text](./Naive%20Forecasting.png)

The Naïve Forecasting is a method of predicting future data based on the last seen data, in this example we use the last value for the train to predict the future of the values following it.

It doesn't do as good as the previous model as this data is seasonal

Notice how it almost performed good in the following month but then wasn't reliable for the data after it. So it's not a very good approach when predicting for the far future.

---

## Comparison
|#  |Model  |RMSE on Train-Test Split | RMSE on k-fold  | RMSE on Roll Forward|
---|--|--|--|--------
|1|Simple Moving Average Smoothing | .. | .. | ..|

## Contributors
|Name                       |Email                              |
----------------------------|------------------------------------
|[Alaa Ali Hassan Sherif](https://www.linkedin.com/in/alaa-sherif/)     |allaashreef00@gmail.com            |
|[Hamsa Wahed Hamed Alawadly](https://www.linkedin.com/in/hamsa-wahed/) |hamsawahed98@gmail.com             |
|[Hebat-Allah Atef Ahmed](https://www.linkedin.com/in/hebat-allah-ahmed/)     |heba.atef.muhammed@gmail.com       |
|[Ishraq Ahmed Jamaluddin](https://www.linkedin.com/in/ishraqahmedjamaluddin/)    |ishraqahmedjamaluddin@gmail.com    |