# Final dataset
https://www.kaggle.com/datasets/taeefnajib/used-car-price-prediction-dataset


The steps
**Midterm:**
1. Exploratory Data Analysis (EDA): you need to understand your data and verify that it doesn't contain errors
- do as much EDA as you can!
2. Split the data into different sets: most often the sets are train, validation, and test (or holdout)
- practitioners often make errors in this step!
- you can split the data randomly, based on groups, based on time, or any other non-standard way if necessary to answer your ML question
3. Preprocess the data: ML models only work if X and Y are numbers! Some ML models additionally require each feature to have 0 mean and 1 standard deviation (standardized features)
- often the original features you get contain strings (for example a gender feature would contain 'male', 'female', 'non-binary', 'unknown') which needs to be transformed into numbers
- often the features are not standardized (e.g., age is between 0 and 100) but it needs to be standardized
--------------------------------------------------------------------------------------------------------
**Final**
4. Choose an evaluation metric: depends on the priorities of the stakeholders
- often requires quite a bit of thinking and ethical considerations
5. Choose one or more ML techniques: it is highly recommended that you try multiple models
- start with simple models like linear or logistic regression
- try also more complex models like nearest neighbors, support vector machines, random forest, etc.
6. Tune the hyperparameters of your ML models (aka cross-validation)
- ML techniques have hyperparameters that you need to optimize to achieve best performance
- for each ML model, decide which parameters to tune and what values to try
- loop through each parameter combination
    - train one model for each parameter combination
    - evaluate how well the model performs on the validation set
- take the parameter combo that gives the best validation score
- evaluate that model on the test set to report how well the model is expected to perform on previously unseen data
7. Interpret your model: black boxes are often not useful
- check if your model uses features that make sense (excellent tool for debugging)
- often model predictions are not enough, you need to be able to explain how the model arrived to a particular prediction (e.g., in health care)