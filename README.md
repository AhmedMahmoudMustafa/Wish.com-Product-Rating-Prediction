# Wish.com Product Rating Prediction

## Problem Formulation:
The goal of this project is to predict the product ratings on Wish.com based on other available features. The input to the model will be various attributes of a product listed on Wish.com, and the output will be the predicted rating of the product. The data mining function required for this task is supervised learning, specifically classification. The challenge lies in dealing with the noisy and unclean dataset, as well as selecting appropriate features and models to achieve accurate predictions. The impact of this project is to provide insights into the factors that contribute to high product ratings and enable estimation of customer satisfaction before listing a product on Wish.com.

## Experimental Protocol:
1. Load the dataset and perform exploratory data analysis (EDA) to gain insights into the data.
2. Preprocess the data by handling missing values, removing duplicates, and addressing any inconsistencies.
3. Perform feature engineering to extract relevant features from the available data.
4. Split the dataset into training and testing sets.
5. Train and evaluate various models using the training set.
6. Tune the hyperparameters of the models to improve their performance.
7. Compare the performance of different models and select the best-performing one.
8. Use the selected model to make predictions on the testing set and evaluate its performance.
9. Iterate on the above steps by trying different feature sets, preprocessing techniques, and model configurations to improve the performance.

## Model Tuning and Documentation:
### Trial 0:
Thoughts and observations:
- The initial dataset contains missing values and noisy data.
- Decision Tree model could be a good starting point for this classification task.
- Plan: Preprocess the data by handling missing values and encoding categorical features. Train a Decision Tree model with default hyperparameters.

### Trial 1:
Thoughts and observations:
- The initial Decision Tree model resulted in overfitting on the training set.
- To address overfitting, the max_depth hyperparameter can be tuned.
- Plan: Train a Decision Tree model with max_depth=5 and compare the performance.

### Trial 2:
Thoughts and observations:
- The Decision Tree model with max_depth=5 performed better than the previous model.
- SVM model can be another option to explore.
- Plan: Train an SVM model with a linear kernel and default hyperparameters.

### Trial 3:
Thoughts and observations:
- The SVM model with a linear kernel showed decent performance, but it might benefit from hyperparameter tuning.
- Plan: Perform grid search to find the optimal hyperparameters for the SVM model.

### Trial 4:
Thoughts and observations:
- The Naive Bayesian model has not been explored yet.
- Plan: Train a Naive Bayesian model and compare its performance with the previous models.
