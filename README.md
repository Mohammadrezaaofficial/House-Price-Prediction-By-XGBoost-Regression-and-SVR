# House-Price-Prediction-By-XGBoost-Regression-and-SVR

## Summary
The document describes a machine learning project focused on predicting house prices using two different regression models: XGBoost Regression and Support Vector Regression (SVR). The dataset used is kc_house_data.csv. The project includes the initial steps of data loading and preparation, followed by the application and evaluation of both models.

## 1. Data Loading and Initial Inspection
The project begins by importing the numpy and pandas libraries. The kc_house_data.csv file is loaded into a pandas DataFrame called df. A statistical summary of the data is presented, showing key metrics for features like price, bedrooms, bathrooms, and various square footage columns (sqft_living, sqft_lot, sqft_above, sqft_basement, sqft_living15, sqft_lot15).The date and price columns are identified as the y (target) variable , while all other columns are treated as x (features). The data is then split into training and testing sets, with 80% of the data used for training and 20% for testing.

## 2. XGBoost Regression
An XGBoost Regressor model is initialized and trained on the pre-processed data. The model's performance is evaluated using the R-squared (R 2 ) metric. The document explains that an R-squared value of 1.0 indicates a perfect prediction, 0 means the model performs no better than predicting the mean, and a negative value means the model is worse than predicting the mean. The trained XGBoost model achieves a training R-squared of 0.99988 and a testing R-squared of 0.89. The document also includes a plot of feature importance for the XGBoost model. The plot shows which features, such as f14, f3, f2, and f15, are most important in determining the predicted house price. It is noted that these features correspond to columns in the feature table, for example f14 is the 14th column of x.

## 3. Support Vector Regression (SVR)
The document then introduces Support Vector Regression (SVR). An SVR model is initialized with a radial basis function (RBF) kernel and other parameters like C=10 and gamma=0.1. The model is trained on a subset of the data (the first 10,000 entries). The document mentions that the predict function is used for making predictions.

## Conclusion
The document successfully demonstrates the application of XGBoost Regression and SVR for predicting house prices. The XGBoost model performs very well, achieving a high R-squared score on both the training and test sets. While the SVR model is introduced and trained, the document does not provide its evaluation metrics, such as R-squared or other scores, so a direct performance comparison between the two models cannot be made from the provided information.
