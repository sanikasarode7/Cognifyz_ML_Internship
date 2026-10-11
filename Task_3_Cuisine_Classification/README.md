# Cuisine Classification

## Project Overview

This project develops a machine learning model to classify restaurants based on their primary cuisine using restaurant-related features. It was completed as part of Task 3 of the Cognifyz Technologies Machine Learning Internship.

## Objective

To build and evaluate a classification model that predicts a restaurant's primary cuisine using available restaurant information.

## Technologies Used

     Python
    Pandas and NumPy
    Matplotlib and Seaborn
    Scikit-learn
    Jupyter Notebook

## Dataset

The project uses restaurant data containing information such as location, average cost, table booking, online delivery, price range, aggregate rating, and votes.

The target variable is the primary cuisine extracted from the restaurant's cuisine information.

## Project Workflow

1. Loaded and inspected the dataset.
2. Checked for missing values and duplicate records.
3. Selected the primary cuisine as the target variable.
4. Prepared numerical and categorical features.
5. Handled missing values using appropriate imputation methods.
6. Excluded cuisine classes with fewer than 20 records.
7. Split the data into training and testing sets using stratification.
8. Encoded categorical variables and scaled numerical features.
9. Trained a Logistic Regression classification model.
10. Evaluated the model using accuracy, macro precision, and macro recall.
11. Analyzed classification performance using a classification report, cuisine recall chart, and confusion matrix.
12. Documented challenges, possible biases, and future improvements.

## Model Evaluation

The current notebook reports the following results:

| Metric | Result |
|---|---:|
| Accuracy | 7.25% |
| Macro Precision | 10.65% |
| Macro Recall | 18.33% |

These results indicate that the current model has limited predictive performance. Further experimentation is required to improve cuisine classification.

## Challenges and Future Improvements

- Imbalanced representation of cuisine classes.
- Limited training examples for less common cuisines.
- Similarities in restaurant features across cuisines.
- Experimenting with Random Forest and other classification algorithms.
- Improving feature selection and addressing class imbalance.

## How to Run

1. Install Python and Jupyter Notebook.
2. Install the required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.
3. Place the dataset in the same folder as the notebook, keeping its filename consistent with the code.
4. Open `Cuisine_Classification.ipynb` in Jupyter Notebook or VS Code.
5. Run all cells from beginning to end.

## Conclusion

The project demonstrates the use of a machine learning classification pipeline for predicting restaurant cuisines. The evaluation highlights the challenges of multi-class classification and identifies areas for future improvement.

## Internship

**Organization:** Cognifyz Technologies  
**Domain:** Machine Learning  
**Task:** Task 3 — Cuisine Classification