# Data Science Portfolio

Repository containing portfolio of data science projects completed by me for academic and self learning purposes.

* ## Project:- Flight Fare Prediction
**Dataset**- Dataset is collected from Kaggle. The dateset is present in [Data_Train.xlsx](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/Data_Train.xlsx).
  
**Problem Statement**- Predict flight fare based on customer’s choice of date, time, airline etc. This will help the customers to plan travel expenses of a trip in advance. 
Dataset contains different flight details of one year to train the model. This is a regression problem.

**Solution**- This dataset has a lot of qualitative variables. I have done a lot of feature engineering to convert them to useful features. This features played important role in training the model. The notebook [DataPreProcessing.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/DataPreProcessing.ipynb) contains all the pre processing steps that are done before training the model. The pre-processed dataset is then stored in the form of pickle file [FlightFareDataFinal.pkl](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/FlightFareDataFinal.pkl). In the next notebook [ML_Model(FlightFare).ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/ML_Model(FlightFare).ipynb), I have tried different algorithms for training the model. After trying different algorithms, I ended up choosing XGBoost. The model is stored in the form of pickle file [Final_XGB_Model.pkl](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/Final_XGB_Model.pkl). For deployment of the model I have used Flask API and the codes are present in the notebook [DeploymentOfModel.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/DeploymentOfModel.ipynb). A webpage is created using HTML codes to show the results. The HTML codes are in [FlightFare.htm](https://github.com/AnannyaPaul/Anannya/blob/main/Flight%20Fare%20Prediction/FlightFare.htm).

**Result**- Using XGBoost I have achieved accuracy of 87.01%. 

* ## Project:- Ecommerce Customer Churn Analysis and Prediction
**Dataset**- Dataset is collected from Kaggle. The dateset is present in [E Commerce Dataset.xlsx](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/E%20Commerce%20Dataset.xlsx).

**Problem Statement**- An online retail (E commerce) company wants to know the customers who are going to churn, so accordingly they can approach customer to offer some promos. This is a classification problem.

**Solution**- This dataset has lot of missing values and outliers which are treated. The target variable is found highly imbalanced. To overcome the effects of imbalanced dataset SMOTE is used. The notebook [DataPreProcessing.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/DataPreProcessing.ipynb) contains all the pre processing steps that are done before training the model. The pre-processed dataset is then stored in the form of pickle file [FinalChurnData.pkl](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/FinalChurnData.pkl). In the next notebook [ML_Model(ChurnPred).ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/ML_Model(Churn%20Pred).ipynb), I have tried different algorithms for training the model. After trying different algorithms, I ended up choosing Random Forest. The model is stored in the form of pickle file [FinalRFModel.rar](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/FinalRFModel.rar). For deployment of the model I have used Flask API and the codes are present in the notebook [DeploymentOfModel.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Ecommerce%20Customer%20Churn%20Analysis%20and%20Prediction/DeploymentOfModel.ipynb).

**Result**- Using Random Forest I have achieved accuracy of 97%. 

* ## Project:- Stock Price Prediction

**Dataset**- The stock data for Infosys has been scraped using nsepy library. The dataset contains the details of a Infosys stock from 2019 to present date.

**Problem Statement**- Predict the closing price of a stock for next day or for the entire week which can be used by traders.

**Solution**- Used closing price of the stock from 2019 to present date to train the model. Shaped the data accordingly before applying LSTM to predict. I have made 2 notebooks. In the notebook [1DayPredAtATime.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Stock%20Price%20Prediction/1DayPredAtATime.ipynb), LSTM is used to predict closing price of the stock for next 1 day at a time. I ran this notebook every morning for a week and then compared the predicted price and original price to calculate the accuracy. In the notebook [5DayPredAtATime.ipynb](https://github.com/AnannyaPaul/Anannya/blob/main/Stock%20Price%20Prediction/5dayPredAtATime.ipynb), LSTM is used to predict closing price of the stock for next 5 days at a time. I ran this notebook at the beginning of the week and then at the end of the week I compared the predicted price and original price to calculate the accuracy. I have used 10 time steps in both the models.

**Result**- The stock market is highly volatile hence predicted for less number of days. When I predicted for 1 day at time, accuracy was 98.28%. When I predicted for 5 days at time, accuracy was 98.24%.

## Support my work 
If you liked what you saw, want to have a chat with me about the portfolio, work opportunities, or collaboration, shoot an email at anannya55paul@gmail.com.
