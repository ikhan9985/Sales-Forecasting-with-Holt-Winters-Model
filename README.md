# Sales Forecasting with Holt-Winters Model
This Flask application performs sales forecasting using the Holt-Winters Exponential Smoothing method on historical sales data stored in an Excel file. It predicts the sales of multiple products and compares the predictions with the actual sales data. The app also provides Mean Squared Error (MSE) metrics and visualizes the predicted vs. actual values in plots.

## Features
- Reads historical sales data from an Excel file.
- Applies the Holt-Winters Exponential Smoothing model to forecast sales.
- Predicts future sales for multiple products over a specified testing period.
- Calculates the Mean Squared Error (MSE) between predicted and actual values.
- Plots the predicted and actual sales values for easy comparison.
- Supports adding trend components (additive) to enhance prediction accuracy.

## Requirements
- Python 3.x

## Libraries:
- pandas
- numpy
- matplotlib
- statsmodels
- scikit-learn

### You can install the required dependencies by running:

pip install pandas numpy matplotlib statsmodels scikit-learn

### Run the Script:
The script automatically reads data from test.xlsx, splits the data into training and testing sets, applies the Holt-Winters model, and makes predictions for each product.
The Mean Squared Error (MSE) is printed for each product along with a comparison of the predicted vs. actual sales during the testing period.
Predicted and actual sales values are visualized using Matplotlib plots.

### Modify the Excel File Path:

If the Excel file is located somewhere other than the script directory, update the file path accordingly:

df = pd.read_excel("path_to_your_file/test.xlsx")


## Output
The script prints the MSE, testing period, and a comparison of predicted vs. actual sales for each product.

### Example output:
Product: Dishwashers
MSE: 73315804.17545429
Testing Period: 2014 to 2018
Predicted vs. Actual:
518633 vs. 525700
538146 vs. 539000

It also shows a plot for each product, visualizing the predicted and actual values over the testing period.

Author Muhammad Imran
