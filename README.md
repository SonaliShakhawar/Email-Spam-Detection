Project Overview
-
This project is a machine learning-based Email Spam Classifier that identifies whether an email is spam or not spam (ham) using TF-IDF Vectorization and a Logistic Regression model.

Problem Statement
-
Email spam is a widespread issue where unwanted messages flood users' inboxes.
Objective: To build a model that accurately classifies emails as spam or not spam based on their content.
Dataset: We use a dataset containing emails labeled as spam (1) and not spam (0).

Tech Stack & Libraries Used
-
Python 
Pandas (for data handling)
--
NumPy (for numerical operations)
--
Scikit-learn (for ML models & vectorization)
--
Jupyter Notebook(for development)
--

Dataset Description
-
The dataset contains two columns:
Message: The text of the email
Category: Label ("spam" or "ham")

Steps Followed in the Project
-
1️ Data Preprocessing
--
Read the dataset using pandas.read_csv().
Replace missing values with empty strings.
Convert labels ('spam' and 'ham') into numerical values (1 for spam, 0 for ham).

2️ Feature Extraction
--
Used TF-IDF Vectorization (TfidfVectorizer) to convert email text into numerical features.
Removed stop words to focus on important terms.
Transformed text data into a matrix for ML training.

3️ Splitting Data
--
Train-Test Split: 80% training, 20% testing using train_test_split().

4️ Model Training 
--
Applied Logistic Regression for classification.
Fit the model using the training data.

5️ Model Evaluation 
--
Predicted spam vs. ham on test data.
Calculated accuracy score to measure performance.
