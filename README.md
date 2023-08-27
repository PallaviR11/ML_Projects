# Analysis of Infant Mortality Rate (IMR) Trends in India

## Introduction

This data science project aims to analyze the trends in Infant Mortality Rate (IMR) across various states and union territories of India from the years 2006 to 2012. The project's objective is to identify patterns, correlations, and insights from the data to gain a better understanding of the factors influencing IMR in different regions.

## Data Collection and Preprocessing

The project utilized a dataset containing information about IMR, state/union territory names, years, and rural/urban classification. The data was loaded into a Pandas DataFrame and underwent preprocessing steps to ensure its quality for analysis.

## Data Exploration and Preprocessing

Null values were managed by removing rows with all NaN values. Additionally, the overall Indian data was dropped from the dataset. A transformed DataFrame was created for further analysis.

## Feature Extraction and Label Encoding

A new DataFrame 'df' was constructed to facilitate model training. This DataFrame included features such as states/union territories, years, and rural/urban classification. State/union territory names were label encoded to convert them into numerical values.

## Data Visualization

- Line Plot: Illustrates the yearly trend of IMR in India, showing a consistent decline over the years.
- Swarm Plot: Represents the distribution of IMR across states/union territories, highlighting differences between rural and urban areas. Notably, IMR is generally higher in rural areas, indicating potential healthcare disparities.

## Data Modeling

Several regression models were applied to predict IMR:
- Linear Regression
- Polynomial Regression (degree = 19)
- Ridge Regression (alpha = 1)
- Decision Tree Regression (max depth = 2)
- K-Nearest Neighbors (KNN) Regression (n_neighbors = 3)
- Bayesian Linear Regression

## Model Evaluation

The models were evaluated using Mean Square Error (MSE) and R-squared (R2) score:
| Model                  | MSE     | R2 Score |
|------------------------|---------|----------|
| Linear Regression      | 189.312 | 0.23218  |
| Polynomial Regression  | 222.243 | 0.09862  |
| Ridge Regression       | 189.334 | 0.23209  |
| Decision Tree Regression | 212.324 | 0.13885  |
| KNN Regression         | 121.781 | 0.13885  |
| Bayesian Linear Regression | 189.432 | 0.23169  |

## Results and Conclusion

- IMR decreased over the years, reflecting advancements in medical care.
- IMR was generally higher in rural areas, highlighting potential healthcare disparities.
- States like Madhya Pradesh, Uttar Pradesh, and Rajasthan exhibited high IMR rates.
- The best-performing model was Bayesian Linear Regression, offering insights for IMR prediction.

## Future Directions

- Explore additional factors contributing to IMR.
- Apply more sophisticated models or ensemble techniques for improved accuracy.
- Conduct geospatial analysis for regional trends.

## References

- [Dataset Source](https://www.kaggle.com/datasets/kaggleprollc/infant-mortality-rate-india-data-collection)

