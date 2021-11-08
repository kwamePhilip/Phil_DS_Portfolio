# Phil_DS_Portfolio
Personal Data Science Projects

# [Project 1: Electrical Energy Predictor: Project Overview](https://github.com/kwamePhilip/electrical_energy_predictor/blob/main/Electrical_Energy_Predictor-1%20(1).ipynb)
* I built a multivariable linear regression model that predicts the net hourly electrical energy output (PE) of a Combined Cycle Power Plant (CCPP) when working with full load.  
* The predictors used in this model are average Ambient Temperature (AT), Ambient Pressure (AP), Relative Humidity (RH), and Exhaust Vacuum (V).
*  A CCPP is typically composed of gas turbines, steam turbines, and heat recovery steam generators
*  I was able to get the model to predict electrical energy output with 92% accuracy on the test data. 
*  A model like this can serve as a Reduced Order Model to help engineers quickly study or troubleshoot a complex system like CCPP with minimal computational resources.
*  Below is a heatmap showing the correlation between variables
*  ![](https://github.com/kwamePhilip/Phil_DS_Portfolio/blob/main/images/heatmap_proj1.png)
*  Below a scatter plot of the models predictions vs the actual test data (y_test)
