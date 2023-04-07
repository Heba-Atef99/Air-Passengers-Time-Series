# Airline Passengers Time Series
This a time series data project that applies all the concepts
![image](https://user-images.githubusercontent.com/54477107/230594840-46483a93-dafc-491c-b48d-0f452c33daa8.png)

# Dependencies
    Python 3.8.10
    Pandas
    NumPy
    statsmodels
    sklearn
    fbprophet
    xgboost

# Evaluation
## Evaluation Metric
We chose RMSE as our evaluation metric
an absolute error measure that squares the deviations to keep the positive and negative deviations from canceling one another out.

![image](https://user-images.githubusercontent.com/54477107/230594578-6fa8ab4f-a28e-4d19-aeeb-69abb3f65fc5.png)

## Data Splitting
### Fixed Train Test Split
![image](https://user-images.githubusercontent.com/54477107/230593907-09967430-b951-4e4e-b5e6-a4ef632198e7.png)

### k-folds Cross Validation
![image](https://user-images.githubusercontent.com/54477107/230593496-f0e40963-2098-4654-870a-b25407eaf890.png)

### Roll Forward
![image](https://user-images.githubusercontent.com/54477107/230594367-03244202-1832-46a3-9160-c8283afddcb6.png)
