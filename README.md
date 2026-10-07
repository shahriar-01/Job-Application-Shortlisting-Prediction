# Job Application Shortlisting Prediction

A machine learning classification project that predicts whether a job applicant will be Shortlisted or Not Shortlisted based on their CGPA, experience, skills, projects, and interview performance.

## Overview

This project uses a synthetically generated dataset to train and compare four classification models:

- Logistic Regression
- Random Forest
- Decision Tree
- K-Nearest Neighbors (KNN)

## Dataset

The dataset is generated inside the notebook (no external files needed) using NumPy with a fixed random seed for reproducibility.

Features:

| Feature | Description |
|---|---|
| cgpa | Academic performance (2.0 - 4.0) |
| experience_years | Years of work experience |
| skill_score | Technical skill test score (0 - 100) |
| projects | Number of completed projects |
| interview_score | Interview performance (0 - 100) |
| shortlisted | Target label (1 = Shortlisted, 0 = Not Shortlisted) |

Samples: 1000
Class distribution: approximately 62% Not Shortlisted, 38% Shortlisted

## Workflow

1. Generate synthetic dataset
2. Exploratory data analysis (EDA)
3. Preprocessing (scaling, train-test split)
4. Train 4 classification models
5. Evaluate using Accuracy, Precision, Recall, F1-score, ROC-AUC, and confusion matrices
6. Compare models and conclude the best fit

## Requirements

numpy
pandas
matplotlib
seaborn
scikit-learn

Install with:

pip install numpy pandas matplotlib seaborn scikit-learn

## How to Run

1. Clone this repository
2. Open the notebook in Jupyter or Google Colab
3. Run all cells from top to bottom

jupyter notebook notebook.ipynb

## Results Summary

All four models are evaluated on the same test set. Logistic Regression and Random Forest perform best overall, as the underlying data pattern is mostly linear. Full metrics, confusion matrices, and ROC curves are available in the notebook.

## Conclusion

Logistic Regression is the most suitable model for this dataset due to strong performance, high stability (low overfitting), and interpretability, which is important for explaining hiring decisions. Random Forest is a close second and a good alternative when prioritizing recall.

## File Structure

project-folder/
  notebook.ipynb   - Main notebook (dataset generation, training, evaluation)
  README.md        - Project documentation
