OBSERVATIONS:
While performing the EDA on the given dataset I observed the following things:
i)The sourcing of the products was mostly done directly
ii)The product type was mainly Powder
iii)There was a dip in the supply from 2020 to 2021
For the same unit of products the Sourcing Cost had a huge variance(outliers)
There were many duplicates of products in the dataset.

APPROACH

Data Pre-processing
1.	Outlier Detection and Removal
o	Used Interquartile Range (IQR) method to detect and remove outliers in sourcing cost data.
2.	Duplicate Removal
o	Removed duplicate rows from the dataset.
3.	Feature Engineering
o	Converted categorical variables into numerical form.
o	Handled missing values using appropriate imputation techniques.
Model Implementation
1.	Feature Selection
o	Separated features (X) and target variable (y) from the dataset.
2.	Data Splitting
o	The entire training dataset was used for model training. This included features (X) and the target variable (y).

o	Similarly, the entire testing dataset was utilized for model evaluation. This allowed for assessing the model's performance on unseen data.

3.	Preprocessing
o	Applied preprocessing steps including imputation and encoding using pipelines and transformers.
4.	Model Training
o	Implemented three regression models: Gradient Boosting, Linear Regression, and Random Forest.
o	Trained each model using the preprocessed training data.
5.	Model Evaluation
o	Made predictions on the testing data for each model.
o	Calculated performance metrics including Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE) to evaluate model performance.
RESULTS
Model Performance
After training and evaluating different regression models on the dataset, the following Mean Squared Error (MSE) values were obtained:
Random Forest:
MSE: 0.009496235817708061
Linear Regression:
MSE: 2.0051432594564256e-08(almost zero)
Gradient Boosting:
MSE:  0.31238480083556425

After comparing the performance of different regression models, Linear Regression stands out as the best-performing model with an extremely low MSE.

Conclusion
This approach encompasses comprehensive analysis of the dataset, preprocessing steps to prepare the data for modeling, and implementation of multiple regression models to predict sourcing costs. The observations from EDA informed the preprocessing steps and model selection process, resulting in a robust analysis of the dataset.

