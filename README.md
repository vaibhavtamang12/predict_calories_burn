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
     ![image](https://github.com/user-attachments/assets/ec28096a-21ef-449c-8bed-1f934b1a91de)

   - Age distrinution
     ![image](https://github.com/user-attachments/assets/87d4fd27-102d-4084-b252-97c1a3004af0)

   - Height Distribution
     ![image](https://github.com/user-attachments/assets/3f97dd0b-a215-4bc2-8179-3a91e9dce04b)

   - Weight Distribution
     ![image](https://github.com/user-attachments/assets/048b7438-fcd4-463b-a40c-04221ea2c8c7)

   - Duration of exercise
     ![image](https://github.com/user-attachments/assets/847929b0-688f-42f4-9e13-718536f8b2ea)

   - Heart Rate Distribution
     ![image](https://github.com/user-attachments/assets/353db4b1-cfd7-4c37-b73a-d24a8f64ee8d)

   - Body Temp.
     ![image](https://github.com/user-attachments/assets/33701e21-417b-4558-b501-26ffbed69e3b)

   - Caloriest Burnt
     ![image](https://github.com/user-attachments/assets/9c1ad6a9-b29d-485b-8876-3f51db9a008c)


4. Bivariate Analysis
   - Gender vs Calories
     ![image](https://github.com/user-attachments/assets/4c403cb2-706a-4f9e-b4e0-9f9da3174803)

   - Age vs Calories
     ![image](https://github.com/user-attachments/assets/736aa53d-92e5-44a2-964b-5216830d65ce)

   - Weight vs Calories
     ![image](https://github.com/user-attachments/assets/da1c3da3-b4d4-4d80-94eb-ab8fc29fc530)

   - Duration of exercise vs Calories
     ![image](https://github.com/user-attachments/assets/79681b90-5837-45a9-9f30-8f4fa1157dfe)

   - Heart_Rate vs Calories
     ![image](https://github.com/user-attachments/assets/19fd4922-4c39-4209-b945-680fec9db17a)

   - Body Temp vs Calories
     ![image](https://github.com/user-attachments/assets/b3179da8-7de4-410d-9182-1ec3b48951eb)

   
5. ML Models
I have trained the dataset on the following models and they gave the respective Root Mean Square Logarithmic Error:

|          Models           |  RMSLE   |
|:------------------------: |:--------:|
| Linear Regression         | **bold** |
| Ridge Regression          |  `code`  |
| Lasso regression          | _italic_ |
| ElsaticNet Regression     | **bold** |
| Decison Tree Regressor    |  `code`  |
| Random Forest Regressor   | _italic_ |
| XGB Regressor             | **bold** |
| LightGBM Regressor        |  `code`  | 
| CatBoost Regressor        | _italic_ |
| KNearest Neighbors        | **bold** |

 
|       Models                  |             RMSLE
|  Linear Regression            |            0.5652
|   
|   Ridge regression                         0.5652
|
|   Lasso regression                         0.5677
|
|   ElasticNet Regression                    0.5842
|
|   Decision Tree regressor                  0.0859
|
|   Random Forest Regressor                  0.0797

   XGB Regressor                            0.0688

   LightGBM                                 0.0684

   CatBoost Regressor                       0.0801

   KNearest Neighbors                       0.6252

The best output is given by LightGbm Regressor with the value of 0.0684
