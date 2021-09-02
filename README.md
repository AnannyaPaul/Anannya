# Data Science Portfolio

Repository containing portfolio of data science projects completed by me for academic and self learning purposes.

## Project:- Flight Fare Prediction
**Dataset**- Dataset is collected from Kaggle. The dateset is present in 'Data_Train.xlsx'.
  
**Problem Statement**- Predict flight fare based on customer’s choice of date, time, airline etc. This will help the customers to plan travel expenses of a trip in advance. 
Dataset contains different flight details of one year to train the model. This is a regression problem.

**Solution**- This dataset has a lot of qualitative variables. I have done a lot of feature engineering to convert them to useful features. This features played important role in training the model. The notebook **'DataPreProcessing.ipynb'** contains all the pre processing steps that are done before training the model. The pre-processed dataset is then stored in the form of pickle file **'FlightFareDataFinal.pkl'**. In the next notebook **'ML_Model(FlightFare).ipynb'**, I have tried different algorithms for training the model. After trying different algorithms I ended up choosing XGBoost. 
