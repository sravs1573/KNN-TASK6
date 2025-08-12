 K-Nearest Neighbors (KNN) on Iris Dataset 

# Overview 
In this task, I implemented the **K-Nearest Neighbors (KNN)** algorithm on the **Iris dataset** to classify flowers into three species: *Iris-setosa*, *Iris-versicolor*, and *Iris-virginica*.  
The project involved **data preprocessing, scaling, model training, evaluation**, and **hyperparameter tuning**. 

# Workflow Steps  

1️ Data Loading & Inspection
- Imported dataset with Pandas.
- Checked data types and confirmed no missing values.
- Dropped `Id` column (not relevant for prediction).

2️ Data Preprocessing
- Scaled features (`SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`) to **0–1** range using **MinMaxScaler**.

3️ Train-Test Split
- Train: 120 samples (80%)  
- Test: 30 samples (20%)

4️ Model Training
- Used KNeighborsClassifier from scikit-learn.
- Initial k value set to 5.

 5️ Model Evaluation
- Test Accuracy:100%  
- Confusion Matrix:
  [[10 0 0]
[ 0 9 0]
[ 0 0 11]]
Classification Report:
              precision    recall  f1-score   support
Iris-setosa       1.00      1.00      1.00        10
Iris-versicolor 1.00 1.00 1.00 9
Iris-virginica 1.00 1.00 1.00 11

Conclusion
-KNN achieved 100% accuracy on the Iris dataset.
-Model performance was unaffected by k value (1–20), indicating a perfectly separable dataset.


