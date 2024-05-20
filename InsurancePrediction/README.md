# Insurance Charges Prediction
The goal of this project is to be able to predict insurance charges, based on a set of variables. This is a regression problem where Linear regression, Ridge regression, Random Forest regressor algorithms were used.
### Exploratory Data Analysis
Of the 7 relevant features, 4 are categorical and 3 are continuous. The target is left skewed, and a strong linear relationship doesn't seem to exist between any of the features and the target; the correlation matrix confirmed it. Nevertheless, the feature smoker and age correlate somewhat to the target.
148 outliers were detected using the interquartile range method.
### Data Preparation
Given the dimensions of the dataset and the nature of the outliers, they were dropped, which didn't affect the statistics of the dataset. The nominal categorical features were transformed into numerical ones.
### Modeling
The dataset was split into a training set and a test set, using the train_test_split method, so that the model could have better performance in unseen data. Three models were chosen: Linear regression, Ridge regression and Random Forest regressor.
### Evaluation
Since this is a regression problem, the evaluation metrics used were accuracy, mean absolute error, and mean squared error.
