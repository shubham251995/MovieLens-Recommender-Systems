# MovieLens Recommender Systems

## Overview
This project explores various recommender system algorithms using the MovieLens 1 Million dataset, focusing on different approaches, including naive methods and advanced matrix factorization techniques. The goal is to predict user ratings for movies based on historical data.

## Dataset
The MovieLens 1 Million dataset consists of approximately 1.007 million ratings provided by around 6,040 users for about 4,000 movies. It's widely used in the recommender systems community for research and benchmarking.

## Methods
### Naive Approaches
- **Global Average**: Predicts ratings based on the overall average rating.
- **Movie Average**: Predicts ratings based on the average rating per movie.
- **User Average**: Predicts ratings based on the average rating per user.
- **Linear Regression**: Two models were tested, one including an error term (gamma) and one without, to predict ratings based on user and movie averages.

### Advanced Techniques
- **UV Matrix Decomposition**: Implemented to explore matrix factorization, aiming to minimize RMSE through iterative optimization.
- **Gravity Recommendation Algorithm**: Applied matrix factorization techniques from the Netflix Prize winners, using parameters like number of factors, iterations, regularization, and learning rate.

## Results
- Various methods were evaluated using k-fold (k=5) cross-validation to ensure robustness and reliability of the results.
- Performance metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error) were used to compare the efficacy of each method.

## Libraries Used
- `pandas` for data manipulation.
- `numpy` for numerical operations.
- `sklearn` for machine learning utilities like cross-validation and error metrics.
- `matplotlib` and `seaborn` for visualizations.
