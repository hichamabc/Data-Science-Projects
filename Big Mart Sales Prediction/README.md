# BigMart-Sales-Prediction

On this project, the purpose is to build a machine learning model that predict the purchase of sales depending on several parameters like  the category of the outlet, the type of the item, the category of the location of the outlet,... this data contains many categorical variables so it is a chance to  use the different techniques of encoding ( OneHotEncoding, LabelEncoding,...)

I build two model, the first is characterised by the fact that the different steps of the model ( cleaning data,feature engineering, building and tuning the model) was done seperately, and the second it is a pipeline which bring all the steps of the project together (using the  make_pipeline module in scikit-learn)

it seems that the second option is very interesting as further the training model  i can evaluate the hole pipeline including the techniques that i choose for the encoding   instead of only evaluating the training model as the case in the first option.

