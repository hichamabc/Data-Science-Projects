# TMDBOX-Dataset-Prediction-of-the-revenues-of-films
TMDBOX Dataset: Prediction of the revenues of films

In this kaggle competition i had the opportunity to work on a subject that excits me a lot since it represent one of my leasure (watching films & series).

The pupose is to predict the revenue of the films, based on different features (popularity,budget, Original language, Production countries,...), it's a regression problem.

This project  envolves many tasks in feature engineering in order to clean  and visualize the data ( for understand it), as many features are stored in paticular data structure : dictionnaries,  for example the crew, cast, gender, languages,....
So i should create multiple function for exctracting the number of crew , of cast  of films by different axes of analysis( by gender, by language,..).

Then i was able to do some exploratory data analysis where i represent especially a comparison between the budget and the revenue of the films through time and by different gender of films,...

For the prediction part i create  two pipeline containing differents steps:
  - PCA( for dimensinality reduction)
  - Gradient Boosting Regressor
  
  the second:
  - Scaling with MinMaxScaler
  - PCA
  - SVR
  
  I didn't use scaling in the first as the algorithm used in tree-based algorithm so scaling is not necessary.
  
  Then i tune the two pipeline using GridSearchCV based on the mean squared logarithmic error as a scoring.
  
  In the end , the first pipeline that have the best score either in train and test scores.
  
  Thanks for reading !
  
