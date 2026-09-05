Comparing The Baseline Performance Of Different Machine Learning Algorithms on Predicting Crop Yield Production
-----------------------------------------------------------

- Dataset (Found On Kaggle):
  ------------------------------

  https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield

  -Dataset had 1,000,000 rows and 10 columns

  -Column names were:
  
    -Region(categorical)
  
    -Soil_Type(categorical)
  
    -Crop(categorical)
  
    -Rainfall(in mm)
  
    -Temperature(celsius)
  
    -Fertilizer_Used(boolean value: true/false)
  
    -Irrigation_Used(boolean value: true/false)
  
    -Weather_Condition(categorical)
  
    -Days_to_harvest
  
    -Yield(in tons per hectare)


- Data Cleaning and Preprocessing:
  --------------------------------------

  -We first converted categorical attributes to Numerical ones using one-hot-encoding.
  
  -We removed Days_to_harvest from the dataset since it was not logical to include it.
  
  -For Algorthms that required finding distances between Data points (like KNN Regression) we first scaled data by using Scikit-Learn Standard Scaler.
  
  -For columns which had Boolean Values(like fertilizer_used  and irrigation_used) we used boolean conversion rules to convert them into 0 and 1's repectively.
  
  -For training we set aside the Yield column for the target variable, (y)



Linear Regression
-------------------------

  -Used Scikit learn LinearRegression Model with no Optimization techniques applied.

  -After testing we calculated the Mean Absolute Error , Mean Squared Error and R^2 error:

    MAE: 0.44158960509232975

    MSE  0.30640508457854443

    r^2 error:  0.8937180917506149

Decision Tree Regressor
------------------------------

    -Used Scikit learn's DecisionTreeRegressor Model with no Optimization techniques applied.
    
    -After testing we calculated the Mean Absolute Error , Mean Squared Error and R^2 error:
    
      MAE: 0.5816531179191097
      
      MSE: 0.5299796954935165
      
      r^2 error; 0.8161673673008519

  
    



