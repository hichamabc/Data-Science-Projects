# Census-Income-Dataset

This project is a particular classification problem, as the data is umbalanced(and high dimensionnal): the amount of samples of the class 1 is too small compared with the class 0.

Explicitly, the purpose is to predict whether the income of a citizen is greater/small than 50K,based on differents informations related to his type of eduction, nationality, race,age, sex, wage per hour,...
 
 So, i begin by doing an exploratory data analysis by the fact of creation some visualization presenting the relation between the output variable and the other variables ( number of individuals of each class by the other variables).
 
 Then it comes the part of feature engineering, as i have in my data many categorical variables , so i need to encode it, i used the label encoding:
 
 i calculate a kind of rate of the wealthy people(>50K) in each category ( number of (>50K)/number of (<50K)) and then i sort those rates, and i change the value of these categories by their index (after sortiong)
 
 
 To cover the problem of imbanlanced data, i proceed with two methods:
 
 - The first is to give the smallest class a greater weight.
 - The second is to use oversampling or preciscely the synthetic minority of oversampling technique(SMOTE from the imblearn module).
 
 Then I trained a gradient boosting classifier , after tuning it using GridSearchCV, i used as metrics the F1-score, as it give a good idea about the precision.recall and how  the model predict good the smallest class
 
 As a result, it seem(from this example) that using the SMOTE is better then change the class weight as in the first case  i have 0.89 as f1 score for the test set,and in the second only 0.6.
 
 Thank you for reading!
 
