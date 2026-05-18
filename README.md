# KNN with scikit-learn - Titanic Classification

## Overview
This project builds a K-Nearest Neighbors (KNN) classifier using the Titanic dataset to predict passenger survival.

## Steps Performed

### 1. Data Preprocessing
- Dropped unnecessary columns: PassengerId, Name, Ticket, Cabin
- Encoded Sex column (male = 1, female = 0)
- Filled missing Age values with median
- Dropped missing Embarked values
- One-hot encoded Embarked column

### 2. Train/Test Split
- Split dataset into training and testing sets (75/25 split)

### 3. Feature Scaling
- Applied StandardScaler to normalize features for distance-based learning

### 4. Model Training
- Trained KNeighborsClassifier from scikit-learn

### 5. Model Evaluation
Metrics:
- Precision: ~0.70
- Recall: ~0.73
- Accuracy: ~0.79
- F1-score: ~0.71

### 6. Hyperparameter Tuning
- Tested multiple values of K 
- Best K found: 17
- Best F1-score: ~0.74

## Conclusion
KNN performed reasonably well on the Titanic dataset. Performance improved after tuning the number of neighbors and scaling features properly.
