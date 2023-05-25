# Air-Quality-Prediction-Using-ARIMA-Model

<p align="center">
  <img src="https://img.shields.io/github/issues/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model" title="logo">
  <img src="https://img.shields.io/github/issues-pr/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model" title="logo">
  <img src="https://img.shields.io/github/forks/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model" title="logo">
  <img src="https://img.shields.io/github/stars/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Modelg" title="logo">
</p>

# About

The air quality index (AQI) is an index for reporting air quality on a daily basis. It is a measure of how air pollution affects one's health within a short time period. The purpose of the AQI is to help people know how the local air quality impacts their health. The Environmental Protection Agency (EPA) calculates the AQI for five major air pollutants, for which national air quality standards have been established to safeguard public health.

1. Ground-level ozone
2. Particle pollution/particulate matter (PM2.5/pm 10)
3. Carbon Monoxide
4. Sulphur dioxide
5. Nitrogen dioxide

The higher the AQI value, the greater the level of air pollution and the greater the health concerns. The concept of AQI has been widely used in many developed countries for over the last three decades. AQI quickly disseminates air quality information in real-
time.

# How is AQI calculated?
India follows that the 500-point scale, wherein rating between 0 and 50 is considered good. Rating between 301 to 500 range is deemed hazardous. Every day monitors record concentrations of the major pollutants. These raw measurements are converted into a separate AQI value for each pollutant (ground-level ozone, particle pollution, carbon monoxide, and sulphur dioxide) using standard formulae developed by EPA. The highest of these AQI values are reported as the AQI value for that day.

# 1. Air Quality Index Categories:
Good (0–50) - Minimal Impact

### 2. Satisfactory (51–100) - 
May cause minor breathing difficulties in sensitive people.

### 3. Moderately polluted (101–200) - 
May cause breathing difficulties in people with lung disease like asthma, and discomfort to people with heart disease, children
and older adults.

### 4. Poor (201–300) - 
May cause breathing difficulties in people on prolonged exposure, and discomfort to people with heart disease.

### 5. Very Poor (301–400) - 
May cause respiratory illness in people on prolonged exposure. Effect may be more pronounced in people with lung and heart diseases.

### 6. Severe (401-500) - 
May cause respiratory issues in healthy people, and serious health issues in people with lung/heart disease. Difficulties may be experienced
even during light physical activity.

### 7. Objectives of Air Quality Index (AQI)

• Comparing air quality conditions at different locations/cities.
• It also helps in identifying faulty standards and inadequate monitoring
programmes.
• AQI helps in analyzing the change in air quality (improvement or degradation).
• AQI informs the public about environmental conditions. It is especially useful for
people suffering from illnesses aggravated or caused by air pollution.

# Motivation behind making the project

When it comes to human health, clean air is the most basic commodity. Today, poor air quality is one of the leading causes of a variety of severe health problems. To estimate the impact on our health, we must be aware of the air quality in our neighborhood, city, and country. The intricate interaction of various components, including chemical reactions, climatic aspects, and emissions from natural and manmade sources, results in air quality. The levels of air pollution in most urban areas have been a source of severe worry. People have the right to know the quality of the air they breathe. However, the data collected by the National Ambient Air Monitoring Network is reported in a format that is difficult to comprehend by the average person, and hence the current air quality
information system does not support people's participation in air quality improvement activities.
The main goal of this project is to investigate the state and quality of the air by measuring the Air Quality Index (AQI) and comparing the measured values to standard values in order to create environmental impact. Therefore, building a forecasting system for predicting the air quality based on the levels of concentration of individual pollutants and various meteorological parameters will be useful for the population’s health.


# GAP AREAS

- The accuracy of the model was found to be unsatisfactory.
- The main reason for the low accuracy is the absence of weather condition data in the model.
- The project did not incorporate weather variables such as temperature, humidity, wind speed and precipitation, which have significant impact on air quality.
- The exclusion of weather conditions limited the model’s ability to capture the complex dynamics and interactions influencing air quality.
- The model’s inability to account for weather-related factors resulted in inaccurate predictions and hindered its effectiveness as a reliable air quality        forecasting tool.
- To enhance the accuracy of future air quality prediction model, it is crucial to integrate weather data to better capture the comprehensive factors affecting   air quality.


# Problem Statement

In this project our main aim is to develop an efficient approach for forecasting the air quality index of Bangalore using meteorological parameters and concentration of major air pollutants using various Machine Learning Algorithms and Deep Neural Networks like LSTM.

# Methodology
1. Data Collection
2. Data Cleaning
3. Data Pre-processing
4. Visualization
5. Training Dataset Formation
6. Model Building
7. Prediction on testing dataset
8. Visualization of predicted model

![flow chart](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/30762db0-3235-40b3-9353-27134d9972fa)

# Data Collection

Concentration of various Air Pollutants like PM2.5, PM10, NO, NO2, NOx, NH3, CO, SO2, O3 were used. Data was collected from Kaggle.

# Data Cleansing

Data cleansing entails identifying incomplete, incorrect, inaccurate, or irrelevant parts of the data and then replacing, modifying, or deleting the dirty or coarse data.

From the data, various features which are not useful in AQI prediction like ‘NH3’, ‘NO’, ‘Benzene’, ‘Toluene’, ‘Xylene’, ‘AQI Bucket’ are removed. Finally, the independent features used are PM2.5, PM10, NO2, NOx, CO, SO2 and O3. Rows with missing AQI values were dropped whereas the missing values in independent
features were interpolated.

# Data Visualization

The data obtained after cleansing was then visualized to check whether the data is proper or not.

![1](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/a1981ab5-4ab0-46b1-baba-4d8c54399c23) <br>
#
![2](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/10ac88a2-edd0-4585-912d-a0003f9bbd7b) <br>
#
![3](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/83278109-7143-46f1-b364-96de4baed3ea) <br>
#
![4](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/60e3d69c-e02d-4776-825e-d258809b2ed9) <br>


# Prediction Result

![prediction AQI 1](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/95ec6fb6-3796-40a7-b3dd-9da8cafec06f) <br>
# 
![p 2](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/18ec6723-c49e-494b-8816-a3b4d55e3ab7) <br>

# Observations

From above, we observed that RMSE is 72.6493297 which is not a good predictions.

# The Influence of Weather Factors on ARIMA Model Performance in AQI Prediction

The ARIMA model is a commonly used technique for time series analysis and forecasting, including air quality index (AQI) prediction. However, it is important to
acknowledge that the accuracy and performance of the ARIMA model can be influenced y various factors, including weather conditions. This note aims to highlight the potential impact of weather factors on the effectiveness of the ARIMA model in predicting AQI values. Weather Factors and AQI: Air quality is significantly affected by weather conditions, such as temperature, humidity, wind speed, and atmospheric pressure. These weather factors can influence the dispersion, formation, and transport of air pollutants, resulting in fluctuations in the AQI. Changes in weather patterns can lead to variations in pollutant concentrations and atmospheric dynamics, which may pose challenges to accurately modeling and predicting AQI using the ARIMA model alone.


Limitations of ARIMA Model in Capturing Weather Effects: The ARIMA model assumes that the underlying time series is stationary and exhibits a linear relationship between past and future values. While it can capture trends, seasonality, and autocorrelation, it may not adequately capture the complex and non-linear relationship between weather factors and AQI variations. The ARIMA model's inability to directly incorporate weather variables as inputs may limit its predictive power, especially in cases where weather plays a significant role in determining air quality.

Importance of Weather-Adjusted Models: To improve AQI prediction accuracy, it is often necessary to consider weather factors explicitly. Weather-adjusted models, such as ARIMA models with weather covariates or more advanced machine learning techniques that incorporate weather data, can be more effective in capturing the influence of weather on AQI. By including weather variables as additional predictors, these models can better account for the impact of temperature, humidity, wind, and other weather-related parameters on air quality dynamics. While the ARIMA model is a valuable tool for time series analysis and forecasting, it may not capture the full complexity of the relationship between weather factors and AQI variations. The influence of weather on air quality highlights the need for advanced modeling techniques that explicitly consider weather data and their interactions with pollutant concentrations. By integrating weather-adjusted models and leveraging comprehensive datasets, we can enhance the accuracy of AQI predictions and gain a better understanding of the complex interdependencies between weather and air quality.

# Hurst Exponent (H)

The Hurst exponent is a mathematical measure used to quantify the long-term dependence or persistence of a time series data. It provides valuable insights into the underlying characteristics and behavior of a dataset, particularly in the context of self- similarity and fractal properties.

The Hurst exponent, often denoted as "H," is named after the British hydrologist Harold Edwin Hurst, who introduced it in the 1950s. It is derived from the concept of fractional Brownian motion and is calculated using various methods, such as the R/S analysis or detrended fluctuation analysis (DFA). The Hurst exponent is a value between 0 and 1, with specific interpretations based on its magnitude:

1. H = 0.5: A Hurst exponent of 0.5 indicates a random or uncorrelated time series.
The data points are independent, and there is no long-term dependence or memory
in the series.

2. H > 0.5: A Hurst exponent greater than 0.5 suggests positive long-term
dependence or persistence. It implies that the time series exhibits a trend or
memory, where past values have a significant influence on future values. The
larger the value of H (> 0.5), the stronger the persistence.

3. H < 0.5: A Hurst exponent less than 0.5 indicates negative long-term dependence or anti-persistence. It implies that the time series tends to revert to the mean or exhibit mean-reverting behavior. Past values have a weaker influence on future values.

![Hurst](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/d17b1986-71bb-41c8-bcff-9f6be027db60)

So, from the above data we can conclude that Hurst exponent is greater than 0.5(mostly) and It implies that the time series exhibits a trend or memory, where
past values have a significant influence on future values.

# Fractal Dimension (D)

Fractal dimension (D) is a measure of the complexity or intricacy of a fractal pattern or object. It quantifies how the detail or structure of a fractal changes as the scale of observation or measurement changes. In short, fractal dimension represents how the object fills or occupies space, exhibiting self-similarity across different scales.

![D](https://github.com/nikki-priyaHIT/Air-Quality-Prediction-Using-ARIMA-Model/assets/66662965/3059b309-083a-46c8-b8a3-4dace7b2b197)

In analyzing the data, it has become evident that the underlying patterns exhibit both multifractal and chaotic characteristics. The presence of multifractality
implies that the data contains multiple scales of variation, with different regions exhibiting distinct degrees of irregularity and complexity.


# Conclusion

The air quality index (AQI) or air pollution index (API) is a standard method of informing the public about the severity of air pollution. Various
researchers/environmental agencies have created a number of ways for determining AQI or API in the past, but there is no globally approved method that is adequate for all scenarios. In computing the AQI or API, different methods utilize different aggregation functions and take into account different types and amounts of contaminants.

When dangerous or excessive quantities of specific chemicals such as gases, particles, and biological molecules are introduced into the atmosphere, it is referred to as air pollution. Excessive emissions have apparent repercussions, such as disease and mortality among populations and other living species, as well as crop damage. Because of the dynamic nature, volatility, and great unpredictability in location and time of pollutants and particles, predicting air quality is a difficult undertaking. Simultaneously, due to the recognized significant repercussions of air pollution on humans and the environment, the ability to model, predict, and monitor air quality is becoming increasingly vital, particularly in metropolitan areas.
