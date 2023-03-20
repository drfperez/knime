# knime
Knime examples for time series forecasting including NYC taxis and energy demand.

Another different workflow is 05_airpollution.knwf. This KNIME workflow come from a paper published on Science Advances at https://advances.sciencemag.org/content/6/45/eabd4049. Reference: Wu, X., Nethery, R. C., Sabath, M. B., Braun, D., & Dominici, F. (2020). Air pollution and COVID-19 mortality in the United States: Strengths and limitations of an ecological regression analysis. Science advances, 6(45), eabd4049.

User car data predicted prices is also interesting to compare predicted prices with algorithms 

Your data will be air pollution time series of a Catalan city, the same city you analysed previously in R.

Steps

1. Data Preparation:
File Reader: Read in the air quality data set.
Column Rename: Rename the columns to be more readable.
String Manipulation: Convert the Date and Time column to a DateTime format.
Missing Value: Handle any missing values.

2. Feature Engineering:
Lag Column: Create lagged versions of the air pollutant data.
Date&Time-based Row Filter: Filter the data for a specific time range.
Joiner: Join the air pollutant data with weather data or other relevant features.

3. Time Series Analysis:
GroupBy: Group the data by date and location.
Time Series Aggregation: Aggregate the air pollutant data into hourly or daily averages.
Time Series to Supervised: Convert the time series data into a supervised learning format.

4. Modeling:
Linear Regression: Fit a linear regression model to the data.
Random Forest: Fit a Random Forest model to the data.
Gradient Boosted Trees: Fit a Gradient Boosted Trees model to the data.
Auto ARIMA: Fit an Auto ARIMA model to the data.
Prophet: Fit a Prophet model to the data.
Recurrent Neural Network: Use an RNN to forecast future air pollutant levels.
Convolutional Neural Network: Use a CNN to classify air pollutant levels.
Autoencoder: Use an autoencoder to detect anomalies in the air quality data.

5. Evaluation:
Regression Scorer: Calculate the Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared for the regression models.
Rule Engine: Apply classification rules to the air pollutant levels and calculate accuracy, precision, and recall.
Confusion Matrix: Visualize the classification results in a confusion matrix.

6. Visualization:
Line Plot: Visualize the actual air pollutant data and the predicted values for each model.
Scatter Plot: Visualize the correlations between different air pollutants.
Heatmap: Visualize the correlation between air pollutants and weather data.
Network Visualization: Generate visualizations of the deep learning models, such as heatmaps of the model's attention or activation maps.

This workflow includes nodes for data preparation, feature engineering, time series analysis, modeling, evaluation, and visualization, covering all of the suggestions I've made. You can customize and modify this workflow based on your specific needs and data.
