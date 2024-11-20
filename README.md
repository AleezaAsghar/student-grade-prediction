# student-grade-prediction

# Student Performance Prediction System

## Overview
This project predicts student performance (Pass/Fail) using a logistic regression model. The model analyzes features like study hours, attendance rate, previous grades, extracurricular participation, and parental education.

## Key Features

- **Preprocessing**:
  - Missing values filled (median for numeric, mode for categorical).
  - Outliers removed using IQR.
  - Categorical variables encoded (label/one-hot encoding).
  - Features scaled with standardization.

- **Model**:
  - Logistic Regression trained on an 80-20 train-test split.
  - Balanced classes using SMOTE (if necessary).



## Usage
1. Load the pretrained model `model.pkl`.
2. Use `preprocessed_data.csv` for evaluation or `testing.ipynb` for predictions.
3. Example prediction:
   - Input: Study Hours: `12.5`, Attendance: `85.0`, Grades: `78.0`.
   - Output: **Pass**.


## Files
- `preprocessed_data.csv`: Preprocessed dataset.
- `model.pkl`: Trained logistic regression model.
- `testing.ipynb`: Script for user input and prediction.


## Future Enhancements
- Use advanced models like Random Forest.
- Incorporate more features for better accuracy.
- Build a user-friendly interface for predictions.
