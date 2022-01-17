# Well_log_ML_project

This project considers prediction of the porosity using well-log data. It contains training and testing different ML models on data from different wells.
After validating the models we can conclude that models trained on a specific well can predict values at other depths for that well with good accuracy. But they poorly generalize for other wells that doesn't take part in the training, since they have different distributions of well-log data.

The best results for the metrics RMSE, MAE and R^2 were shown by the XGBoost regressor and LSTM model (that consider time-series by depth).

notebooks:
* well_log_ml_models.ipynb - training ml models (RF, XGBoost, KNN, Linear Regression, FNN) and testing them on different wells
* well_log_feature_engineering.ipynb - feature engineering + training and testing ml models on the transformed data
* well_log_time_series.ipynb - training and testing time series model (RNN)
* well_log_time_series_feature_eng.ipynb - feature engineering of the sequential data (by depth) and training/testing RNN model

Data for different wells (170, 169, 171, 183 PL) are give in the 'data/' dir

Authors:
Ilya Nachinkin  
Ramilya Sharifullina  
Gladchenko Elizaveta
