# House Price Prediction Using Machine Learning

## Overview
This project applies data science techniques to analyze housing sales data and build a predictive model for home prices. Using **exploratory data analysis (EDA)**, **feature engineering**, and **multiple regression models**, we identify key factors influencing home prices and develop a predictive model.

## Key Features
- **Data Cleaning & Preprocessing:**
  - Handled missing values through imputation and filtering.
  - Standardized numeric features and encoded categorical variables.
  - Created new engineered features like `price_10000` and `renovated`.
- **Exploratory Data Analysis (EDA):**
  - Analyzed distributions, outliers, and correlations.
  - Visualized trends in house prices based on `sqft_living`, `grade`, `view`, etc.
- **Predictive Modeling:**
  - **Multiple Linear Regression** models built and evaluated.
  - Considered interactions between key variables (e.g., `bedrooms:bathrooms`).
  - Best-performing model achieved **R² = 0.6557**, explaining ~65.57% of price variance.
- **Model Evaluation:**
  - Used **RMSE** (Root Mean Squared Error) to assess prediction accuracy.
  - Compared multiple models, selecting the best trade-off between complexity and accuracy.

## Technologies Used
- **R** (tidyverse, dplyr, tidymodels, ggplot2, lubridate, factoextra, mosaic, cluster)
- **R Markdown** for report generation
- **GitHub** for version control and collaboration

## Results
- **Key Features Influencing Home Prices:**
  - `sqft_living`, `grade`, `view`, `waterfront`, and `bathrooms` were among the most predictive variables.
  - `sqft_living` had the highest correlation with price.
- **Best Model (Model 7a):**
  - Included key predictors, interactions, and transformations.
  - Achieved **RMSE = 46.88** on test data.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/house-price-prediction.git
   ```
2. Open **RStudio** and install required libraries:
   ```r
   install.packages(c("tidyverse", "tidymodels", "mosaic", "factoextra", "lubridate", "cluster"))
   ```
3. Run the analysis by opening **Final project II.Rmd** in RStudio and knitting the report.

## Future Work
- Explore more complex models like Random Forest or Gradient Boosting.
- Include geographic data for neighborhood-based analysis.
- Improve feature engineering for better model performance.

## Contributors
- **Gerard Corrales**

## License
This project is licensed under the MIT License - see the LICENSE file for details.
