# Predict Used Vehicle Price

## Project Overview

This project focuses on building and evaluating machine learning models to predict the price of used vehicles using historical listing data. The workflow covers data exploration, preprocessing, outlier removal, feature engineering, model comparison, and final price prediction.

The objective of this project is to demonstrate practical data science and machine learning skills, including exploratory data analysis (EDA), regression modeling, performance evaluation, and model comparison.

---

## Dataset Description

The dataset contains used vehicle listings with the following key features:

- **Price** – Target variable (vehicle selling price)
- **Year** – Manufacturing year
- **Mileage** – Distance driven
- **Make** – Vehicle brand
- **Model** – Vehicle model
- **City** – Listing city
- **State** – Listing state

The data was analyzed to understand pricing trends across states, manufacturers, and vehicle characteristics.

---

## Exploratory Data Analysis (EDA)

The project includes:

- Checking for missing values
- Distribution analysis of vehicle prices (top 1% removed to reduce skewness)
- Average price analysis by top 10 states
- Average price analysis by top 10 car manufacturers
- Crosstab analysis of state and car make distribution
- Box plots to detect outliers

Outliers were removed using the Interquartile Range (IQR) method to improve model accuracy.

---

## Data Preprocessing and Feature Engineering

To prepare the data for modeling:

- Categorical variables (Model, City, State) were converted into numeric representations
- Outliers were removed using IQR
- The dataset was split into training and testing sets
- Feature scaling was applied where necessary

---

## Machine Learning Models Implemented

The following regression models were trained and evaluated:

1. Linear Regression  
2. Polynomial Regression  
3. Spline Regression  
4. Random Forest Regressor  

---

## Model Evaluation

Models were evaluated using:

- **R-squared (R²)** – Measures how well the model explains variance
- **Root Mean Squared Error (RMSE)** – Measures prediction error magnitude

### Performance Comparison

| Model                 | R² Score | RMSE     |
|-----------------------|----------|----------|
| Linear Regression     | 0.44     | 7185.69  |
| Polynomial Regression | 0.54     | 6501.54  |
| Spline Regression     | 0.54     | 6498.24  |
| Random Forest         | 0.86     | 3522.48  |

Random Forest achieved the best performance, demonstrating strong predictive capability compared to the other models.

---

## Price Prediction Example

The project demonstrates how to predict vehicle prices using new input data.

Example input format:




The trained model generates predicted prices based on these features.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

---

## Project Structure





---

## Key Learnings

- Proper data cleaning and outlier removal significantly improve model performance.
- Tree-based models such as Random Forest perform better than simple linear models for complex pricing datasets.
- Feature engineering and exploratory data analysis are critical before modeling.
- Comparing multiple algorithms provides better insight for model selection.

---

## Future Improvements

- Deploy the model as a web application
- Perform hyperparameter tuning
- Use cross-validation for more robust evaluation
- Implement advanced models such as XGBoost or LightGBM
- Add feature importance visualization

---

## Author

Shoyeb Ahmmed  
Computer Science Graduate  
Data and Machine Learning Enthusiast
