# Insurance_Cost_Prediction
# Context:-
It is a supervised learning model that can predict the cost of premium for health insurance, i.e predict the continous data / numerical Value
# Project_Analysis:-
Machine learning algorithms can predict the cost of the premium for health insurance. The cost of the premium for health insurance varies from person to person. For example, a smoker is charged higher premium than a non-smoker. Companies calculate the premium for each person based on few factors like age, bmi, smoker etc. It is possible to predict the premium cost using machine learning algorithms. We can train a machine learning algorithm using the past data to predict the premium cost and make a model.

The size of dataset is 1338 records. It contained 7 columns, out of which six of them was independent variable and one was dependent variable. The data was labeled so we can do supervised learning algorithms. As the dependent variable is continuous numerical value this is a regression problem. The data contains no missing values but it does contain outliers.

However, some machine learning algorithms like decision tree and random forest are not sensitive to outliers, therefore we have not removed the outliers. The variables have good correlation except for regions. The variables like bmi, children and smoker are normally distributed but the others are not. Feature scaling using min-max scaler was done to give all features equal importance and scale them in the range of 0 to 1. Different ml algorithms were trained using the dataset and tested.

Random Forest gave the best r2 score of 85.25% and adjusted r2 score of 85.19% as well both are close enough but has difference in them .According to the theory the r2 score is greater than adjusted r2 score i,e (Adjusted R2 is always less than or equal to R2) shows good model.

We also use hyperparameter tuning on Random forest using GridSearchCV that gives 84.58% and RandomizedSearchCV that gives 84.00% that is less than the normal Random Forest .

We trained the Decision tree Algorithm again with best parameters.The r2 score increased to 85.43% and adjusted r2 score was 85.20%. Again it shows r2 score is greater than the adjusted r2 score.

At the last we conclued that Decision Tree Algorithm shows the best accuracy/performace among all the others algorithm for this model.
