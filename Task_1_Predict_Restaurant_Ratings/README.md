# Predict Restaurant Ratings

## Project Overview

This project uses machine learning to predict the aggregate rating of a restaurant based on its available features. It was developed as Task 1 of the Cognifyz Technologies Machine Learning Internship.

## Objective

To build a regression model that predicts restaurant aggregate ratings using restaurant-related data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses a restaurant dataset containing 9,551 records and 21 columns. The dataset includes restaurant details, location, cuisine, cost, services, votes, and aggregate ratings.

## Implementation

1. **Dataset Inspection:** Loaded the dataset and examined column names, data types, missing values, duplicate records, and sample rows.
2. **Data Preprocessing:** Handled missing cuisine values by replacing them with `Unknown`.
3. **Feature Selection:** Selected `Aggregate rating` as the target variable and excluded `Rating color` and `Rating text` from the input features.
4. **Feature Identification:** Separated categorical and numerical features.
5. **Categorical Encoding:** Applied One-Hot Encoding to categorical features using `OneHotEncoder` with `handle_unknown="ignore"`.
6. **Train-Test Split:** Divided the data into 80% training data and 20% testing data using `random_state=42`.
7. **Model Training:** Trained a Linear Regression model.
8. **Model Evaluation:** Evaluated predictions using Mean Squared Error (MSE) and R-squared (R²).
9. **Feature Analysis:** Examined regression coefficients to identify features with the largest absolute coefficient values.
10. **Visualization:** Created an Actual vs Predicted Ratings scatter plot.

## Model Evaluation Results

| Metric | Result |
|---|---:|
| Mean Squared Error (MSE) | 1.7577 |
| R-squared (R²) | 0.2277 |

The MSE measures the average squared prediction error, while R² indicates the proportion of rating variation explained by the model. The R² result indicates that the model explains approximately 22.77% of the variation in the test data.

## Conclusion

A Linear Regression model was developed to predict restaurant aggregate ratings. The model was evaluated using MSE and R², and its results were examined through a scatter plot and regression coefficient analysis. The results indicate that further improvements to feature selection, preprocessing, and model selection may help improve prediction performance.

## How to Run

1. Install Python and Jupyter Notebook.
2. Install the required libraries: `pandas`, `numpy`, `matplotlib`, and `scikit-learn`.
3. Place the dataset file named `Dataset .csv` in the same folder as the notebook.
4. Open the notebook in Jupyter Notebook or VS Code.
5. Run all cells from beginning to end.

## Internship Details

- **Organization:** Cognifyz Technologies
- **Domain:** Machine Learning
- **Task:** Task 1 — Predict Restaurant Ratings