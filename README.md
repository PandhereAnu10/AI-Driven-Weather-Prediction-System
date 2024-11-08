# AI-Driven-Weather-Prediction-System

## NASA Space Weather Analysis

This project uses the NASA Open Data API to fetch space weather data, specifically Coronal Mass Ejections (CMEs), and analyze it with Python. It visualizes the frequency of CME events over time and makes future predictions using Facebook's Prophet model. The repository contains the code and necessary instructions to replicate the analysis.

## Table of Contents
- Requirements
- Setup
- Usage
- Data Fetching and Processing
- Visualization
- Forecasting with Prophet
- Model Evaluation
- Results
- License

## Requirements
To run this code, you need the following libraries:

- ```requests```
- ```pandas```
- ```matplotlib```
- ```prophet``` (requires ```pystan```)

Install them with:

`
pip install requests pandas matplotlib prophet
`

## Setup
1. Get a <a href="https://api.nasa.gov/">NASA Open Data API Key (DONKI)</a> .
2. Replace `API_Key` in the code with your NASA API key.

## Usage
1. Run the code to fetch CME data from NASA's API.
2. The data is cleaned and visualized to show the frequency of events over time.
3. A time-series model predicts future CME events.

## Data Fetching and Processing
The data is fetched from NASA’s DONKI (Database of Notifications, Knowledge, Information) API. The data is then converted into a DataFrame for analysis.

## Visualization
Two main visualizations are created:

- Bar Plot: Shows the number of CME events on each date.
- Line Plot: Shows the number of CME events over time.

## Forecasting with Prophet
The code uses the Prophet model to:

- Forecast CME event frequencies for the future.
- Plot the forecasted results with actual data for comparison.
  
## Model Training
The data is split into training and testing sets, with 80% for training. The Prophet model is fit on the training data, and future dates are predicted.

## Model Evaluation
To evaluate the forecast accuracy, we calculate the Mean Absolute Error (MAE), comparing actual vs. predicted values.

## Results
The final plot displays actual and predicted CME event occurrences, helping assess the model’s accuracy.


