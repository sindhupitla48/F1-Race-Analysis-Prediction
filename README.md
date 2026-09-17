
# F1 Race Points Prediction Using Machine Learning

## Project Overview

This project focuses on predicting Formula 1 driver race points using Machine Learning.

Historical Formula 1 race data from 2010 to 2024 was cleaned, processed, and analyzed to identify patterns in driver and team performance.

## Objectives

- Analyze historical Formula 1 race data
- Clean and preprocess the dataset
- Arrange races in chronological order
- Correct invalid duplicate race positions
- Create historical and rolling performance features
- Prevent data leakage
- Train and compare Machine Learning models
- Predict driver race points
- Analyze prediction errors

## Dataset

- Years: 2010–2024
- Number of races: 300
- Drivers per race: 20
- Total records: 6,000
- Final columns: 39
- Target variable: Points

## Data Preprocessing

- Chronological race ordering was created.
- Invalid duplicate race positions were corrected.
- Start, qualifying, and finish positions were validated.
- Duplicate rows were checked.
- Historical driver and team features were created.
- Rolling performance features were created.
- Championship points before each race were calculated.
- Historical features were created using previous-race information to reduce data leakage.

## Machine Learning Models

The following regression models were compared:

1. Linear Regression
2. Gradient Boosting
3. Random Forest
4. Decision Tree

## Model Comparison

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 5.041 | 6.778 | 0.257 |
| Gradient Boosting | 5.102 | 6.835 | 0.239 |
| Random Forest | 5.359 | 6.951 | 0.213 |
| Decision Tree | 5.925 | 8.246 | -0.108 |

## Best Model

Linear Regression was selected as the final model.

Final chronological test performance:

- MAE: 5.041
- RMSE: 6.778
- R²: 0.257

## Data Split

- Training data: 4,800 records
- Testing data: 1,200 records
- Training races: 1–240
- Testing races: 241–300

## Visualizations

The project includes:

- Actual vs Predicted Points
- Model Comparison
- Prediction Error Distribution
- Average Prediction Error by Driver

## Project Structure

F1_Race/

- Kaggle_Source.pdf
- data/
- models/
- notebooks/
- visualizations/
- README.md

## Limitations

F1 race outcomes can be affected by unpredictable factors such as crashes, safety cars, penalties, weather, and race strategy.

The current model explains a limited portion of the variation in race points.

## Future Improvements

- Circuit-specific performance
- Practice-session data
- Weather forecasts
- Sprint race results
- Grid penalties
- Driver and constructor championship position
- Tire compound information
- Hyperparameter optimization
- Advanced Machine Learning models

## Conclusion

This project demonstrates how Machine Learning can be used to analyze historical Formula 1 data and predict driver race points.

After data cleaning, chronological ordering, feature engineering, leakage prevention, and model comparison, Linear Regression achieved the best test performance with MAE 5.041, RMSE 6.778, and R² 0.257.
