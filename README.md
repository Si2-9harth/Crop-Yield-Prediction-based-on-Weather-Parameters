# Crop Yield Prediction based on Time Series Forecasting of Weather Parameters

Did time series forecasting of weather parameters such as rainfall, temperature etc. for districts all over Chhattisgarh, India using stacked LSTM and then predicted the crop yield using various regression models. 

# Data Preperation ->
The datasets available were seperately available which were converted to dictionaries and fed to the final dataset which looked like this ->
![image](https://user-images.githubusercontent.com/98142436/162388271-76409b8d-20ab-4cc8-a860-d0de7ecd1d1a.png)

To make the data more up to date we used stacked LSTM to learn from the data of previous years that is the weather parameters and predicted weather parameters for 1 year 
which would be used in prediction of crop yield.

# Pipeline Used ->
1. Train Test Split was done with keeping test size to 25%.
2. Feature Selection using Mutual Info Regression and F Regression was done.
    Result from Mutual Info Regression ->
    ![image](https://user-images.githubusercontent.com/98142436/162388989-7b007e0c-e405-46a1-81ae-2c3139b99d63.png)
3. Fitting algorithms by using all the features and practicing scaling and using MAE for validation.
![image](https://user-images.githubusercontent.com/98142436/162389316-1db4f8de-600a-4fa0-bec3-6452731b4239.png)
4. Crop Production plots ->
![image](https://user-images.githubusercontent.com/98142436/162389481-0257d456-cbbf-40c6-9d2d-d5d343356c13.png)
![image](https://user-images.githubusercontent.com/98142436/162389503-54f15609-7480-4ac3-8f9b-44952e94f864.png)
Since target variable is skewed the Log Transformation was being used.
5. Keras built deep neural networks were also used to get the best model for prediction.

![image](https://user-images.githubusercontent.com/98142436/162389728-12a4ce5f-29af-4a4e-8657-6b7e16479000.png)

6.Final Output on Rabi Crops ->
![image](https://user-images.githubusercontent.com/98142436/162389891-44740056-3890-479a-a175-105cf130d026.png)
