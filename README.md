# CO2 Emission Prediction using Linear Regression

## Objective

This project uses **Linear Regression** to predict **CO2 emissions** from a car based on its **engine size** and **fuel consumption** (mileage). The aim is to find how these factors affect the emission of carbon dioxide and build a simple predictive model.

## Dataset

The dataset contains:
- `ENGINESIZE` (in liters)
- `FUELCONSUMPTION_COMB` (combined fuel usage, L/100 km)
- `CO2EMISSIONS` (grams/km - our target)

## Methodology

1. **Data Cleaning**
   - Missing values were handled (if any).
   - Selected only useful columns for prediction.

2. **Feature Selection**
   - First model: used only `ENGINESIZE`
   - Second model: used both `ENGINESIZE` and `FUELCONSUMPTION_COMB`

3. **Splitting**
   - Used `train_test_split` to divide data into 80% training and 20% testing.

4. **Model Building**
   - Used `LinearRegression()` from `sklearn` to create a regression model.
   - Trained the model using `.fit(X_train, y_train)`

5. **Results**
   - The coefficients and intercept of the regression line were printed.
   - These define the equation for predicting CO2 emissions.



