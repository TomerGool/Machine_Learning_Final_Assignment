# Machine_Learning_Final_Assignment
Introducing the learning problem A corpus data (labeled database) of stories (corpus labeled, i.e. includes target values). Each story has a tag • 'm –' for writer (male) • 'f' - for a female writer. We build a classification model whose function is to classify the gender of a narrative paragraph as above.

# Text Classification Preprocessing and Model Evaluation
This repository contains code for a text classification assignment involving preprocessing text data, training machine learning models, and evaluating their performance using F1 scores. The goal of the assignment is to build a pipeline that takes raw text data, preprocesses it, trains multiple classification models, and predicts the categories of test examples.

# Assignment Steps
Text Cleaning and Preprocessing:
The provided text data undergoes cleaning and preprocessing, which involves removing digits, punctuation, and extra whitespace. The cleaned text is then stored in pandas DataFrame objects.

# Train-Test Split:
The cleaned training data is split into training and testing sets for both features and target labels. This step ensures that we have data for training and evaluating our models.

# TF-IDF Vectorization:
The cleaned text data is transformed into numerical features using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. This process converts the text data into a format suitable for machine learning algorithms.

# Feature Selection:
Mutual information scores are calculated to select the most important features. This step helps reduce the dimensionality of the data while retaining relevant information.

# Feature Scaling:
The selected features are scaled using the MaxAbsScaler to maintain the sparsity structure of the data. This step ensures that features are on a similar scale, which can improve model performance.

# Model Selection and Hyperparameter Tuning:
Various classification models (e.g., LinearSVC, Perceptron, Multinomial Naive Bayes, MLP, SGD) are trained using the preprocessed and scaled training data. Hyperparameter tuning is performed using GridSearchCV to find the best combination of hyperparameters for each model.

# Model Evaluation:
The trained models are evaluated using cross-validation and F1 scores. The fit_predict_evaluate function is used to fit the models, predict on the test set, and calculate F1 scores. The F1 scores are calculated separately for each gender category and then averaged.

# Test Data Prediction:
The best-performing model (SGD) is used to predict the categories of the provided test examples. The test data undergoes the same preprocessing steps as the training data, and the predictions are stored in a pandas DataFrame.
