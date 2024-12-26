# Stroke_prediction

Dataset Loading and Preprocessing:

Loaded the stroke dataset.
Handled missing values in the bmi column using median imputation.
Applied one-hot encoding to categorical features: gender, marital status, work type, residence type, and smoking status.
Handled the outliers in the 'avg_glucose_level' column
Scaled numerical features (age, average glucose level, and BMI) using StandardScaler.

Feature Selection:
Used SelectKBest to identify the top 10 most relevant features for prediction.

Class Imbalance Handling:
Applied SMOTE (Synthetic Minority Oversampling Technique) to oversample the minority class (stroke cases).

Data Splitting:
Split the dataset into training and testing sets.

Model Training and Evaluation:

Trained three models:
Logistic Regression
Random Forest
XGBoost

Used RandomizedSearchCV for hyperparameter tuning.

Evaluated model performance using:
Accuracy
Classification report
ROC AUC scores
Confusion matrices

Custom Stroke Risk Prediction:
Created a function to make stroke risk predictions based on user-provided input data.
