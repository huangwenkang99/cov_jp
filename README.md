# ReadMe

[87582eae-361c-448a-9442-e4d6ce24bcf8_Data.csv],[confirmed_cases_cumulative_daily.csv],[number_of_deaths_daily.csv],[vaccination_data5.xlsx] are the original files. [reshaped_economic_data.csv],[daily_average_confirmed_cases_no_decimal_corrected.csv],[yearly_vaccination_totals.csv] are the files that are reshaped by extracting the data from the original files

This repository contains the cov_jp_2.py script, which analyzes the impact of the COVID-19 pandemic on Japan's economy and public health using historical data. The script examines the relationships between key economic indicators, such as GDP growth rate and unemployment rate, and COVID-19 confirmed cases for the years 2021 to 2023. It also predicts future trends for the years 2024 to 2026 using a linear regression model.

Features
Data Processing: The script loads, cleans, and processes data from multiple sources, including vaccination totals, confirmed COVID-19 cases, and economic indicators.
Data Visualization: The script generates plots to visualize the relationship between economic and public health variables, including:
Actual GDP growth rate vs. Unemployment rate
Actual COVID-19 confirmed cases
Predictive Modeling: The script uses a linear regression model to predict:
Future GDP growth rates
Future unemployment rates
Future confirmed COVID-19 cases
Text Output: The script outputs the actual and predicted values for key indicators, providing a clear summary of both historical data and forecasted trends.
Data Sources
Vaccination Data: Contains yearly totals of vaccinations administered in Japan.
Confirmed Cases Data: Includes yearly confirmed COVID-19 cases in Japan.
Economic Data: Includes various economic indicators such as GDP growth rates and unemployment rates, reshaped for analysis.

Prerequisites
Python 3.x
Required Python packages: pandas, matplotlib, scikit-learn, numpy
You can install the required packages using pip:

pip install pandas matplotlib scikit-learn numpy

Usage
Load Data: The script loads data from CSV files provided in the repository.
Data Processing: The script processes the data by removing duplicates, handling missing values, and merging datasets based on the 'Year' column.
Data Visualization: The script generates visual plots to analyze historical data (2021-2023) and predicted data (2024-2026).
Modeling and Prediction: The script trains a linear regression model using historical data and makes predictions for future years.
Running the Script
To run the script, use the following command:

python cov_jp_2.py

Output
Text Output: The script outputs the actual and predicted values for GDP growth rates, unemployment rates, and confirmed COVID-19 cases for the specified years.
Plots: The script generates plots comparing actual and predicted data.
Example Output

Actual Values (2021-2023):
Year: 2021
  Actual GDP Growth Rate: X.XX%
  Actual Unemployment Rate: Y.YY%
  Actual Confirmed Cases: ZZZZZZ

Predicted Values for 2024-2026:
Year: 2024
  Predicted GDP Growth Rate: X.XX%
  Predicted Unemployment Rate: Y.YY%
  Predicted Confirmed Cases: ZZZZZZ


Acknowledgments
Data Sources: Ministry of Health, Labor and Welfare of Japan, and the World Bank database.
Inspiration: This project was inspired by ongoing efforts to understand the economic and public health impacts of the COVID-19 pandemic and to forecast future trends.
