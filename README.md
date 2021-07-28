# HackerEarth-HourlyTrafficVolume_Prediction-99.96755_Accuracy
**Time series regression model to predict the hourly traffic volume in metro city for the next 1.5 years using train data for past 5 years**
***
![Prediction score using XGBoost with FT](https://github.com/Qadir92/HackerEarth-HourlyTrafficVolume_Prediction-99.96755_Accuracy/blob/main/Traffic%20score.PNG?raw=true)
***
**Steps in the notebook:**
 1. Loading the data into colab notebook.
 2. Convert 'date_time' column in datetime format.
 3. Dickey Fuller Test on the series to confirm **series is stationary**.
 4. Use **feature engineering** to derive new columns **'Hour', 'Day', 'Month', 'Year', 'weekday', 'non_working', 'time_of_day'** and *ordinal encoding* for *'weather_type'* with 'Squall', 'Fog', 'Thunderstorm', 'Smoke', 'Mist', 'Snow', 'Clear', 'Drizzle', 'Rain', 'Clouds', 'Haze' in ascending order.
 5. Training statsmodel and sklearn Linear Regression and plotting the actual vs predicted traffic volume.
 6. Using **RMSE** and **MAE** for measuring accuracy of the models.
 7. Dropping the 'is_holiday', 'air_pollution_index', 'humidity', 'wind_speed', 'wind_direction', 'dew_point','temperature', 'rain_p_h', 'snow_p_h', 'clouds_all', 'weather_description', 'Day', 'weekday' features from the dataframe.
 8. Add **Fourier term** on year, week and day in the time series.
 9. Training the **Elastic Net** and **XGBoost** model and Elastic Net and XGBoost with **Fourier Terms.**
 10. Hyper tuning **XGBoost with Fourier terms** model.
 11. Predictions using XGBoost tuned with Fourier terms.
***
To check out my notebook, please click [here](https://github.com/Qadir92/HackerEarth-HourlyTrafficVolume_Prediction-99.96755_Accuracy/blob/main/Traffic_Volume_Forecasting.ipynb)

*Reload the notebook couple of times to get the preview*
