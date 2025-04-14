Heart Disease Prediction System
Project Overview
This machine learning project predicts the likelihood of heart disease based on patient health metrics such as age, cholesterol levels, and blood pressure. The system uses Support Vector Machine (SVM) for classification and includes comprehensive preprocessing steps to ensure reliable predictions.

Dependencies
Make sure to install the following Python libraries:

pandas - For data manipulation and analysis.

numpy - For numerical computations.

scikit-learn - For machine learning algorithms and preprocessing.

matplotlib & seaborn - For data visualization.

Optional: imbalanced-learn for handling class imbalance if necessary.

Data Preprocessing
Handling Missing/Null Values:

Drop rows with insignificant missing values or use k-nearest neighbors imputation for missing health metrics like cholesterol or blood pressure.

Feature Engineering:

Combine metrics such as age, cholesterol (chol), and resting blood pressure (trestbps) into risk indices if needed for better modeling performance.

Label Encoding:

Encode categorical variables like chest pain type (cp) into numerical values using one-hot or label encoding.

Normalization/Standardization:

Scale numerical features using StandardScaler to ensure all features contribute equally to model performance.

Model Training
Train-Test Split:

Split the dataset into 70% training data and 30% testing data with random shuffling.

Support Vector Machine (SVM):

Use the SVM classifier with a polynomial kernel to capture non-linear relationships in the data.

Optimize hyperparameters like degree of polynomial kernel, regularization parameter (C), and gamma using grid search.

Building the Predictive System
Develop a function that accepts patient health metrics (e.g., age, cholesterol levels, resting ECG results).

Preprocess inputs using the same pipeline applied during training.

Use the trained SVM model to predict heart disease risk levels ("Low Risk," "High Risk").
