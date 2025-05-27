# predict_calories_burn
Kaggle competition for May 2025 where we have to predict Calories burned using ML models and calculate their root mean square logarithmmic error

1. Understanding the Dataset:

   - There are 2 integer columns, 6 float value columns and 1 object column

   - There are 750000 rows and 9 columns
  
2. Data Quality Checks:

   - There are 0 null values

   - There are no duplicates in the dataset

   - There is a high correlation between the following columns:
   
     1. Height and Weight
   
     2. Duration of Exercise and Heart Rate

     3. Duration of Exercise and Body Temp.

     4. Duration of Exercise and Calories burned

     5. Body Temp. and Heart Rate

     6. Heart rate and Calories Burned

     7. Body Temp. and Calories Burned

   - There are outliers in height, weight, heart_rate, body_temp and calories columns.

3. Univariate Analysis

   - Sex Count
   - Age distrinution
   - Height Distribution
   - Weight Distribution
   - Duration of exercise
     ![image](https://github.com/user-attachments/assets/de421454-8e5e-4f0f-9a7f-4a61ab61d268)

   - Heart Rate Distribution
   - Body Temp.
   - Caloriest Burnt

4. Bivariate Analysis
   - Gender vs Calories
   - Age vs Calories
   - Height vs Calories
   - Weight vs Calories
   - Duration of exercise vs Calories
   - Heart_Rate vs Calories
   - Body Temp vs Calories

   
5. ML Models
I have trained the dataset on the following models and they gave the respective Root Mean Square Logarithmic Error:
 
        Models                               RMSLE
   Linear Regression                        0.5652
   
   Ridge regression                         0.5652

   Lasso regression                         0.5677

   ElasticNet Regression                    0.5842

   Decision Tree regressor                  0.0859

   Random Forest Regressor                  0.0797

   XGB Regressor                            0.0688

   LightGBM                                 0.0684

   CatBoost Regressor                       0.0801

   KNearest Neighbors                       0.6252

The best output is given by LightGbm Regressor with the value of 0.0684
