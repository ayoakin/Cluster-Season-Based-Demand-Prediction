# Dartmouth Machine Learning Project Team 5

Project Objective: Predicting Bike Sharing Demand in Seoul
Our project aims to develop and evaluate machine learning models to predict bike sharing demand in Seoul using the UCI dataset. By analyzing hourly bike rental patterns in relation to weather conditions and temporal factors, we seek to create accurate prediction models that can help optimize bike sharing operations.

Dataset Overview
The dataset contains 8,760 hourly observations (representing one full year from 12/2017 to 11/2018) with 14 features:

| Variable                | Variable Description                        | Type  |
|-------------------------|-------------------------------------------|-------|
| Date                    | The day of the 365 days                    | str   |
| Rented Bike Count       | Number of rented bikes                     | int   |
| Hour                    | The hour of the day                        | int   |
| Temperature (C)         | Temperature of the day                     | float |
| Humidity                | Humidity in the air                        | int   |
| Wind speed (m/s)        | Speed of wind                              | float |
| Visibility (10m)        | Visibility in range of 10m                 | int   |
| Dew point temperature (C)| Temperature at the start of the day       | float |
| Solar radiation (MJ/m²) | Solar radiation per unit on horizontal area| float |
| Rainfall (mm)           | Amount of rainfall                         | float |
| Snowfall (cm)           | Amount of snowfall                         | float |
| Seasons                 | Season of the year                         | str   |
| Holiday                 | If it is a holiday                         | str   |
| Functioning day         | if it is a function day                    | str   |

The dataset is complete with no missing values, providing a solid foundation for our predictive modeling work.

Research Foundation

Our project builds upon existing research, particularly:
- Jelic (2021): Achieved 92% accuracy using Autoregression models
- Sathishkumar & Cho (2020): Demonstrated success with Random Forest algorithms

Project Objectives

Primary Objective
- Develop a model to accurately predict the hourly “Rented Bike Count” using available features
- Target performance should aim to match or exceed previous benchmarks (92% accuracy)
- Handle the wide range of demand (0 to 3,556 bikes per hour)

Analytical Focus Areas
1. Understand how different factors affect bike sharing usage:
   - Weather conditions (temperature, humidity, precipitation)
   - Temporal patterns (hour of day, day of week)
   - Seasonal variations (Winter, Spring, Summer, Autumn)
   - Special conditions (holidays vs. regular days)
2. Compare different machine learning approaches:
   - Random Forest
   - Autoregression
   - Other potential methods (gradient boosting, neural networks)
   - Ensemble approaches

Technical Objectives
- Implement proper train-test splitting considering the temporal nature of the data
- Handle data preprocessing needs (scaling, encoding categorical variables)
- Evaluate models using multiple metrics (R², RMSE, MAE)
- Consider developing separate models for different seasons if needed
Practical Applications
- Provide interpretable results to understand feature importance
- Create models that can be used for operational planning
- Consider both short-term (hourly) and medium-term (daily/weekly) predictions
- Focus on operational days (when Functioning Day = ‘Yes’)
- Help bike sharing operators better predict and manage fleet distribution
Methodology Approach
1. Exploratory Data Analysis
   - Analyze distribution of the target variable (Rented Bike Count)
   - Examine correlations between features
   - Visualize seasonal and temporal patterns
2. Feature Engineering
   - Create time-based features (day of week, month)
   - Handle categorical variables
   - Consider interaction terms between weather variables
3. Model Development
   - Implement multiple modeling approaches
   - Tune hyperparameters for optimal performance
   - Validate models using cross-validation
4. Evaluation and Interpretation
   - Compare model performance across different conditions
   - Identify key predictive factors
   - Provide actionable insights for bike sharing operations