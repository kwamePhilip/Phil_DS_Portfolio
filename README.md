# Phil_DS_Portfolio
Personal Data Science Projects

# [Project 1: Electrical Energy Predictor: Project Overview](https://github.com/kwamePhilip/electrical_energy_predictor/blob/main/Electrical_Energy_Predictor-1%20(1).ipynb)
* I built a multivariable linear regression model that predicts the net hourly electrical energy output (PE) of a Combined Cycle Power Plant (CCPP) when working with full load.  
* The features used in this model are average Ambient Temperature (AT), Ambient Pressure (AP), Relative Humidity (RH), and Exhaust Vacuum (V).
*  A CCPP is typically composed of gas turbines, steam turbines, and heat recovery steam generators
*  I was able to get the model to predict electrical energy output with 92% accuracy on the test data. 
*  A model like this can serve as a Reduced Order Model to help engineers quickly study or troubleshoot a complex system like CCPP with minimal computational resources.
*  Below is a heatmap showing the correlation between variables
*  ![](/images/heatmap_proj1.png)
*  Below is a scatter plot of the models predictions vs the actual test data (y_test)
*  ![](/images/pred_vs_ytest.png)
*  
# [Project 2: Water Potability Predictor: Project Overview](https://github.com/kwamePhilip/water_potability_predictor/blob/main/Water%20Potability%20Predictor%20(1).ipynb)
*  Potability of water indicates if the water is safe for human consumption. Here, 1 = Potable and 0 = Not Potable
*  My goal in this project was to compare several classification models to find the one that predicts the potability of water with highest accuracy and lowest False Positves
*  The classification models I compared were Extreme Gradient Boosting (XGBoost), Gradient Boosting (GBoost), Random Forest, and K Nearest Neighbors (KNN)
*  I used SciKit learn's *GridSearchCV* to perform the hyperparameter tuning
*  The dataset was obtained from kaggle.com and contains nine water quality metrics for 3276 different water bodies
*  **XGBoost** model predicted the water potability with **79%** accuracy. Below is the plot of the Confusion Matrix for the XGBoost model
*  ![](/images/xgboost_CM.png)
*  **Random Forest** model predicts the water potability with **78%** accuracy. Below is the plot of the Confusion Matrix for the Random Forest model
*  ![](/images/RF_CM.png)
*  **Gradient Boosting** model predicts the water potability with accuracy score of **80%**. Below is the plot of the Confusion Matrix for the Gradient Boosting model
*  ![](/images/GB_CM.png)
*  **KNN** model predicts the water potability with accuracy score of **63%**. Below is the plot of the Confusion Matrix for the KNN model
*  ![](/images/knn_CM.png)
*  The Gradient Boosting model is the best not only because it has the highest accuracy but has the lowest false positives percentage.
*  Because a false poisitive by this model will be very catastrophic, I will select the model with lowest percentage of false positive and highest recall score.  Therefore, **Gradient Boosting** wins!
*  A plot of feature importance from the Gradient Boost model is shown below
*  ![](/images/impt_feat_gb.png)
*  The **sulfate concentration** and **pH** are the top two most important features in determining the potability


