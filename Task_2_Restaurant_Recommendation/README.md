# Restaurant Recommendation System

## Project Overview

This project implements a content-based restaurant recommendation system that suggests restaurants according to user preferences. It was developed as Task 2 of the Cognifyz Technologies Machine Learning Internship.

## Objective

To recommend restaurants based on user preferences, particularly cuisine and price range, using content-based filtering.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- SciPy
- Matplotlib
- Jupyter Notebook

## Dataset

The project uses a restaurant dataset containing 9,551 records and 21 original columns. A subset of seven columns is selected for recommendations: Restaurant ID, Restaurant Name, Cuisines, Price range, City, Aggregate rating, and Votes.

## Implementation

1. **Dataset Inspection:** Loaded the dataset and examined its columns, missing values, duplicate records, and sample data.
2. **Feature Selection:** Selected restaurant names, cuisines, price ranges, cities, aggregate ratings, and votes for the recommendation dataset.
3. **Data Preprocessing:** Handled missing cuisine, price range, restaurant name, and city values.
4. **Duplicate Handling:** Removed duplicate records based on Restaurant ID.
5. **Preference Selection:** Defined cuisine preference and price range as the recommendation criteria.
6. **Cuisine Encoding:** Used TF-IDF Vectorization to represent cuisine information numerically.
7. **Price Encoding:** Applied One-Hot Encoding to the price range.
8. **Feature Matrix:** Combined cuisine and price-range features into a single feature matrix.
9. **Content-Based Filtering:** Used cosine similarity to compare user preferences with restaurant features and rank restaurants.
10. **Recommendation Testing:** Tested the system using North Indian cuisine and price range 2, generating the top 10 recommendations.
11. **Quality Evaluation:** Evaluated the recommendations using cuisine match rate, price-range match rate, and overall preference match rate.
12. **Visualization:** Created charts showing recommendation similarity scores and the price-range distribution of recommended restaurants.

## Sample User Preferences

| Preference | Value |
|---|---|
| Preferred cuisine | North Indian |
| Preferred price range | 2 |
| Number of recommendations | 10 |

## Recommendation Quality Results

For the sample preferences tested in the notebook:

| Evaluation Metric | Result |
|---|---:|
| Cuisine Match Rate | 100% |
| Price Range Match Rate | 100% |
| Overall Preference Match Rate | 100% |

These results indicate that all 10 recommendations matched the selected cuisine and price range according to the notebook's evaluation criteria. They apply to this sample query and do not establish recommendation quality for every possible user preference.

## Conclusion

A content-based restaurant recommendation system was developed using TF-IDF, One-Hot Encoding, and cosine similarity. The system ranks restaurants according to cuisine and price-range preferences and evaluates the resulting recommendations using matching percentages. Similarity scores and price-range distributions are also visualized to help interpret the results.

## How to Run

1. Install Python and Jupyter Notebook.
2. Install the required libraries: `pandas`, `numpy`, `scikit-learn`, `scipy`, and `matplotlib`.
3. Place the dataset file named `Dataset .csv` in the same folder as the notebook.
4. Open the notebook in Jupyter Notebook or VS Code.
5. Run all cells from beginning to end.

## Internship Details

- **Organization:** Cognifyz Technologies
- **Domain:** Machine Learning
- **Task:** Task 2 — Restaurant Recommendation