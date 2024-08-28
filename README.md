# cov_jp
Overview
This Python program analyzes the relationship between COVID-19 confirmed cases, vaccination data, and economic indicators (GDP growth rate and unemployment rate) in Japan from 2020 to 2023. Using a linear regression model, the program forecasts GDP growth rates, unemployment rates, and confirmed COVID-19 cases for the years 2024 to 2026. The results are visualized through a series of plots, which allow for a deeper understanding of the interplay between the pandemic and economic recovery.

Prerequisites
Before running this program, ensure you have the following Python packages installed:

pandas
statsmodels
matplotlib
sklearn
numpy
You can install these packages using pip:

bash
pip install pandas statsmodels matplotlib scikit-learn numpy
Datasets
The program requires the following datasets to be available in CSV format:

Vaccination Data: yearly_vaccination_totals.csv
Confirmed Cases Data: yearly_confirmed_cases.csv
Economic Data: reshaped_economic_data.csv
Ensure that the datasets are correctly formatted and located in the appropriate directory.

Program Workflow
Loading Data: The program loads vaccination, confirmed COVID-19 cases, and economic data from the respective CSV files.

Data Cleaning and Preparation:

Duplicates in the economic data are removed.
The economic data is pivoted to have one column per economic indicator (e.g., GDP growth, unemployment rate).
The datasets are merged based on the Year column.
Missing values are handled by replacing them with NaN and using forward fill.
Data Filtering: The merged dataset is filtered to include data from 2020 to 2023.

Visualization:

Plot 1: Compares the unemployment rate and GDP growth rate from 2020 to 2023.
Plot 2: Compares the GDP growth rate and confirmed COVID-19 cases from 2020 to 2023.
Plot 3: Compares the unemployment rate and confirmed COVID-19 cases from 2020 to 2023.
Linear Regression Model:

The program uses a linear regression model to predict GDP growth rates based on the unemployment rate and confirmed COVID-19 cases.
The model is trained on data from 2020 to 2023.
Forecasting (2024-2026):

The program predicts GDP growth rates, unemployment rates, and confirmed COVID-19 cases for the years 2024 to 2026.
The predicted values are displayed in a DataFrame.
Prediction Visualization:

Group 1: Plots the predicted GDP growth rate and unemployment rate for 2024 to 2026.
Group 2: Plots the predicted confirmed COVID-19 case rate for 2024 to 2026.
Usage
Ensure the required datasets are in the correct directory.
Run the Python script using the following command:
bash
python your_script_name.py
The program will display the plots and predicted values in the console.
Output
Predicted Values (2024-2026): The program will output a DataFrame containing the predicted GDP growth rate, unemployment rate, and confirmed COVID-19 cases for the years 2024, 2025, and 2026.
Plots: The program generates several plots to visualize the actual and predicted relationships between the pandemic and economic indicators.
Data Sources
The data used in this program is sourced from:

Ministry of Health, Labor and Welfare of Japan
World Bank Database
License
This program is open-source and free to use under the MIT License. You are free to modify, distribute, and use the code as needed.

Contact
For any questions or issues, please contact the developer at [s2022011@stu.musashino-u.ac.jp].
