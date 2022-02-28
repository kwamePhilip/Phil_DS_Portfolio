# Phil_Projects
Personal Machine Learning Projects

# [Project 2: Water Potability Predictor: Project Overview](https://github.com/kwamePhilip/water_potability_predictor/blob/main/Water%20Potability%20Predictor%20(1).ipynb)
*  Potability of water indicates if the water is safe for human consumption. Here, 1 = Potable and 0 = Not Potable
*  My goal in this project was to compare the performance metrics of several classification models that predicts the potability of water.
*  The classification models I compared were Extreme Gradient Boosting (XGBoost), Gradient Boosting (GBoost), Random Forest, and K Nearest Neighbors (KNN).
*  The dataset was obtained from kaggle.com and contains nine water quality metrics for 3276 different water bodies.
*  After selecting a final model (**Gradient Boosting**), I deployed the model with a Flask application (link below).
*  [https://water-potability-test.herokuapp.com/](https://water-potability-test.herokuapp.com/)
*  **Gradient Boosting** model predicts the water potability with accuracy score of **80%**. Below is the plot of the Confusion Matrix for the Gradient Boosting model.
*  ![](/images/GB_CM.png)
*  The Gradient Boosting model is the best not only because it has the highest accuracy but has the lowest false positives percentage.
*  Because a false poisitive by this model will be very catastrophic, I will select the model with lowest percentage of false positive and highest recall score.  Therefore, **Gradient Boosting** wins!
*  A plot of feature importance from the Gradient Boost model is shown below.
*  ![](/images/impt_feat_gb.png)
*  The **sulfate concentration** and **pH** are the top two most important features in determining the potability.

#  [Project 3: Recycled Water Conductivity Predictor (ANN vs MLR models): Project Overview](https://github.com/kwamePhilip/Conductivity_Predictor_from_IOT-_sensors/blob/5dcce5023b760250b458e6306bea3d7c7c438b95/Water_Conductivity_Predictor_from_IOT_Sensing_Data.ipynb)
*  Water conductivity is directly related to the concentration of ions in the water. These ions come from dissolved salts and other inorganic materials.
*  In this project, I compared the **Root Mean Squared Errors (RMSEs)** of **Artificial Nueral Network (ANN)** and **Multivariable Linear Regression (MLR)** models in predicting the **Conductivity** of Recycled Water.
*  The observations used in this model were recorded from IOT sensors.
*  The bar plot below shows the features and how they correlate with the target variable (Conductivty).
*  ![](/images/conductivity_corr.png)
*  The **RMSEs** of both the **ANN** and **MLR** are **29.2** and **28.8** respectively. Therefore, there is no significant difference in the performance of both models.
*  In this case the **MLR** will be selected since it requires lesser computational resources, faster, and can be easily deployed.
*  Below is the scatterplot of the Actual Conductivity Test data vs the Predicted Conductivity data.
*  ![](/images/Conductivity_pred_vs_test.png)
*  Models like this one can be used by scientists for chemistry control studies and also use to check for possible sensor or analytical errors in a data.

# [Project 1: Electrical Energy Predictor: Project Overview](https://github.com/kwamePhilip/electrical_energy_predictor/blob/main/Electrical_Energy_Predictor-1%20(1).ipynb)
* I built a **multivariable linear regression** model that predicts the net hourly **electrical energy output (PE)** of a Combined Cycle Power Plant (CCPP) when working with full load.  
* The predictors used in this model are average **Ambient Temperature (AT)**, **Ambient Pressure (AP)**, **Relative Humidity (RH)**, and **Exhaust Vacuum (V)**.
*  A CCPP is typically composed of gas turbines, steam turbines, and heat recovery steam generators.
*  I was able to get the model to predict electrical energy output with **92%** accuracy on the test data. 
*  A model like this can serve as a Reduced Order Model to help engineers quickly study or troubleshoot a complex system like CCPP with minimal computational resources.
*  Below is a heatmap showing the correlation between variables.
*  ![](/images/heatmap_proj1.png)
*  Below is a scatter plot of the model's predictions vs the actual test data (y_test).
*  ![](/images/pred_vs_ytest.png)





