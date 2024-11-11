# DocAssist
Building Intelligent Medical Decision Support System
Objective: Build a model to aid in making informed decisions for the best treatment options for individual patients.

Data Import: Load the dataset containing medical parameters from an Excel file.

Initial Data Exploration:

Display dataset shape, head, info, and summary statistics.
Examine data distributions across parameters like HAEMATOCRIT, HAEMOGLOBINS, ERYTHROCYTE, LEUCOCYTE, THROMBOCYTE, and AGE using histograms.
Data Preprocessing:

Separate features (X) from the target label (y) labeled as SOURCE.
Convert categorical variable SEX to binary (1 for male, 0 for female).
Data Splitting: Divide the data into training and testing sets (90% train, 10% test).

Save Datasets: Export the training and testing sets into CSV files for reproducibility.

Model Selection: Choose a Random Forest Classifier to classify patients based on medical features.

Hyperparameter Tuning:

Define a parameter grid for tuning the model’s complexity, tree depth, number of estimators, and sampling.
Use RandomizedSearchCV with cross-validation to identify the best hyperparameters.
Model Training: Fit the model on the training data with optimized parameters.

Model Evaluation:

Make predictions on the test set and calculate accuracy.
Also assess accuracy on the training set to check for overfitting.
Save Model: Store the trained model using joblib for future use.

Precision Evaluation:

Calculate and print precision scores for both the test and train sets, providing insight into prediction reliability.
