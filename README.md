# Walmart-sales-forecasting
The model chosen for this project is the Random Forest Regressor(n_estimators, max_depth, max_features). It is an ensemble method and uses multiples decision trees ('n_estimators' parameter of the model) to determine final output, which is an average of the outputs of all trees

We will use BoxCox (Boxcox1p from scipy.special) to understand if there is change of correlation and skewness for some features against target variable. In some cases, transforming a variable can help, depending on the model, if skewness changes or correlation seem to change with different values of lambda. We can decide to drop the variable if no change is observed.


Boxcox1p(x, lambda) : ((1+x)^lambda -1) / lambda | if lambda != 0   
                       log(1+x)                  | if lambda == 0

