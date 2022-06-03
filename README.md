# SantanderCustomerTransactionPrediction
 ## Identify which customers will make a specific transaction in the future
 <br /> Throughout this project, I was trying to find out if there is a way to determine which customers will make a specific transaction in the future, irrespective of the amount of money transacted.<br />
 <br /> The Python Libraries that have been used for this project including **Numpy, Pandas, sklearn, scipy, skopt, matplotlib, xgboost, lightgbm, tensorflow and bayes_opt.**
 <br />
 <br /> After understanding the business background and the problem statement, I started exploring the dataset doing **basic EDA**. There were 200k observations and 200 features in the training dataset and same size for the testing data. Considering all these 200 features, I needed to find the most relevant features that help to make better predictions. <br />
 <br />The next step was **feature engineering** since the features that went into the model are crucial for training a good prediction model. Then I checked for missing values and repeated values and found that there wass none of them.<br />
 <br />After the above, I started to try different models including **Logistic Regression, Random Forest, XGBoost and LightGBM**. After comparing these models, I decided to stick with **LightGBM**. Finally after all algorithms have been validated, trained and tested, I ended up using LightGBM model with the help of **Bayesian Optimization** to **pick the best hyperparameters** and **Stratified K Fold** to elevate the **AUC score** on our validation dataset. After the model being built, by plotting the feature importance among all the features I had, I knew the weighted contribution of each feature to final predictions.

