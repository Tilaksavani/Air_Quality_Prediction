# ML_Project-Air Quality Prediction Project 🌫⚠️☠️

Air pollution poses a significant risk to health, and accurate prediction of air quality can help mitigate its harmful effects. This project aims to predict air quality levels using Python and machine learning algorithms.

## Prerequisites

This project requires Python 3.6 or higher, along with the following Python libraries:

- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [matplotlib](https://matplotlib.org/)
- [scikit-learn](https://scikit-learn.org/)
- [seaborn](https://seaborn.pydata.org/)

It’s recommended to install [Anaconda](https://www.anaconda.com/products/distribution) as it comes pre-installed with most of these libraries.

### Installing Dependencies

To install the required libraries, you can use pip:

```bash
pip install numpy pandas matplotlib scikit-learn seaborn
```

Additionally, you will need to install [Jupyter Notebook](https://jupyter.org/) to run the code and visualize the results.

## Project Files

This repository includes the following files:

- `Speckbit_Project_Air_Quality_Prediction(T).ipynb`: Main notebook for air quality prediction.
- `Speckbit_Project_Air_Quality_Prediction[C6H6(GT)].ipynb`: Alternative model for predicting C6H6(GT).
- `AirQualityUCl.csv`: The dataset with air quality readings from multiple sensors.

## How to Run the Project

To get started, navigate to the project directory and open the Jupyter notebook with the following command:

```bash
jupyter notebook Air_Quality_Prediction_Using_ML(Output-T).ipynb
```

or
```
jupyter notebook Air_Quality_Prediction_Using_Machine_Learining(Output-C6H6).ipynb
```

## Dataset Information

The dataset contains sensor readings from a chemical multisensor device located in a highly polluted area of an Italian city. The data was collected hourly over the span of one year (March 2004 to February 2005).

### Dataset Details:

- 9358 instances of hourly data from five metal oxide chemical sensors.
- Data includes readings for CO, Non-Methanic Hydrocarbons (NMHC), Benzene, NOx, and NO2.
- Ground truth data for these pollutants is provided by a reference analyzer.
- Missing values are tagged with **-200**.

### Features:

- **Date**: Date in DD/MM/YYYY format
- **Time**: Time in HH:MM:SS format
- **CO Concentration**: CO concentration (mg/m³, from reference analyzer)
- **PT08.S1 Sensor Response**: Sensor response for CO (nominally CO targeted)
- **NMHC Concentration**: Non-Methanic Hydrocarbons concentration (µg/m³, from reference analyzer)
- **Benzene Concentration**: Benzene concentration (µg/m³, from reference analyzer)
- **PT08.S2 Sensor Response**: Sensor response for NMHC (nominally NMHC targeted)
- **NOx Concentration**: Nitrogen Oxides concentration (ppb, from reference analyzer)
- **PT08.S3 Sensor Response**: Sensor response for NOx (nominally NOx targeted)
- **NO2 Concentration**: Nitrogen Dioxide concentration (µg/m³, from reference analyzer)
- **PT08.S4 Sensor Response**: Sensor response for NO2 (nominally NO2 targeted)
- **PT08.S5 Sensor Response**: Sensor response for O3 (nominally O3 targeted)
- **Temperature**: Temperature (°C)
- **Relative Humidity**: Relative Humidity (%)
- **Absolute Humidity**: Absolute Humidity (AH)

### Target Variables:

- **C6H6**: Ground truth concentration for Benzene (target variable)
- **T**: Temperature (target variable)

## Machine Learning Models Used

This project employs the following machine learning models to predict air quality:

1. **Linear Regression**: A simple model that establishes a relationship between the input features and the target variable.
2. **Lasso Regression**: A variant of linear regression that applies L1 regularization to enhance model generalization.
3. **Decision Tree Regression**: A non-linear model that splits the data based on different decision rules to predict the target variable.

These models are trained to predict the concentration of pollutants, based on the sensor data and environmental factors provided in the dataset.

## How to Use

1. Download the dataset `AirQualityUCl.csv` and place it in the project directory.
2. Open the Jupyter notebook and follow the steps in the code to preprocess the data, train the models, and evaluate their performance.
3. Use the trained models to make predictions on new data and analyze the air quality levels.
