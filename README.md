Fraud Detection with PySpark

This project aims to detect fraudulent transactions using PySpark, a powerful analytics engine for large-scale data processing. The dataset used for this project is the credit card fraud detection dataset.

Flow of the project

Environment Setup

•	Install PySpark by running !pip install pyspark.

•	Mount Google Drive to access the dataset by running from google.colab import drive and drive.mount('/content/drive').

Dataset

•	Ensure the dataset (creditcard.csv) is located in your local machine.

•	Load the dataset into the PySpark DataFrame.

Exploratory Data Analysis (EDA)

•	Perform basic EDA such as viewing the data, checking schema, and counting missing values.

•	Visualize class distribution to understand the imbalance in the dataset.

Data Preprocessing

•	Balance the dataset by undersampling the majority class and creating a balanced DataFrame.

•	Assemble features and label using VectorAssembler.

Model Building

•	Train multiple machine learning models including Random Forest, Logistic Regression, Decision Tree, Gradient Boosted Trees, and Linear SVC.

•	Evaluate model performance using Area Under ROC (AUC) metric.

•	Compare AUC scores of different models without using pipeline.

Pipeline Implementation

•	Implement a pipeline to streamline the preprocessing steps including vectorization and scaling.

•	Train the same models using the pipeline.

•	Evaluate model performance and compare AUC scores with the non-pipeline approach.

Hyperparameter Tuning

•	Perform hyperparameter tuning for Random Forest, Logistic Regression, Decision Tree, Gradient Boosted Trees, and Linear SVC using CrossValidator.

•	Find the best hyperparameters for each model.

•	Re-train the models with the optimized hyperparameters.

•	Evaluate model performance and compare AUC scores with and without hyperparameter tuning.

Visualization

•	Visualize AUC scores of different models using bar plots.

•	Compare AUC scores of models with and without pipeline, as well as with hyperparameter tuning.

Conclusion

This project demonstrates the implementation of fraud detection using PySpark, from data loading to model evaluation. Through experimentation with various models and techniques such as pipeline and hyperparameter tuning, the goal is to achieve the highest possible AUC score for accurate fraud detection.
