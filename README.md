
# Univariate Load Forecasting
The aim is to use immenent features in Univariate analysis, and demonstrate a comparision based on two different analogy of rolling feature.
Hourly Electrical Load data(Kw) of 31 users is used for forecasting.
First, the user with worst pattern to learn is selected by creating multiple models and testing each user with it.
Once the target user is selected, we have created a model and concatenated the data of all other 30 users to train our model with various profiles. 
Result: The model performs well with 10 estimators and default hyperparameters when using Random Forest.(The model is not optimised for excellence Yet)
## Result of forecasting using general rolling features and 6 temporal features

![alt text](https://github.com/amitt00/Load_Forecasting/blob/main/Result%20Images/Univariate_30Feature_result.png)
## Result of forecasting same data with featureset 2 (27 features)
![alt text](https://github.com/amitt00/Load_Forecasting/blob/main/Result%20Images/Univariate_27Feature_result.png)


# MultiVariate Load analysis
The aim is to forecast the load of given panama country.
Dataset: Dataset is taken from kaggle and pre processed
LSTM is used as a base model for forecasting. To improve the results bayesian optimisation is used and the result is shown via graph in code.

## Forecasting result before using bayesian
![alt text](https://github.com/amitt00/Load_Forecasting/blob/main/Result%20Images/beforebayesian_MultiVariate.png)

## Forecasting result after setting optimum hyper parameters using bayesian optimisation along with the training/test loss over epochs

![alt text](https://github.com/amitt00/Load_Forecasting/blob/main/Result%20Images/loss_Multivariate_afterBayesian.png)
![alt text](https://github.com/amitt00/Load_Forecasting/blob/main/Result%20Images/AfterBayesian_MultiVariate.png)
