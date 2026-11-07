# AI-Based SNR Prediction Using Machine Learning

## Project Overview

This project focuses on predicting the Signal-to-Noise Ratio (SNR) of wireless communication networks using environmental and communication-related parameters.

Machine learning regression algorithms are implemented to analyse the relationship between environmental conditions, communication measurements, and wireless signal quality.

The project is based on the research paper:

**"SNR Prediction Based on Environmental Sensing Data: An Approach Using Machine Learning" (2025)**

Authors: Kanchanarat Chokruay and Anya Apavatjrut.

## Objectives

- Predict wireless SNR using machine learning.
- Analyse the influence of environmental parameters on signal quality.
- Compare multiple regression algorithms.
- Evaluate model performance using standard regression metrics.
- Develop an interactive SNR prediction demonstration.

## Dataset

The project uses the publicly available LoRaWAN dataset:

[LoRa RSSI Dataset – GitHub](https://github.com/emanueleg/lora-rssi)

Dataset source: Vineyard-2021.

The dataset includes:
- Temperature
- Humidity
- Atmospheric pressure
- Rainfall
- RSSI
- SNR
- Soil temperature
- Soil humidity
- Battery measurements
- Communication parameters

Eight LoRaWAN sensor nodes are included.

## Methodology

1. Dataset exploration and analysis.
2. Missing-value investigation and data cleaning.
3. Timestamp alignment and hourly aggregation.
4. Integration of environmental and sensor datasets.
5. Exploratory Data Analysis.
6. Feature engineering and selection.
7. Machine learning model development.
8. Model evaluation and comparison.
9. Interactive SNR prediction demonstration.

## Machine Learning Algorithms

The following regression algorithms were implemented:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

## Model Performance

Random Forest achieved the best performance in our chronological test-set evaluation.

| Metric | Result |
|---|---:|
| MAE | 0.1600 |
| MSE | 0.0437 |
| RMSE | 0.2090 |
| R² Score | 0.7083 |

The model was evaluated using an 80:20 chronological train-test split.

## Technology Stack

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib

## Interactive Demonstration

An interactive prediction interface allows users to enter environmental and communication parameters and obtain an estimated SNR value.

## Repository Contents

- `SNR_Prediction_ML_Implementation.ipynb` – Complete implementation, preprocessing, model training, evaluation and prediction interface.
- Additional model files, results and visualisations will be added as the project is organised.

## Research Note

The reported model performance represents our implementation and evaluation on the selected dataset. It should not be interpreted as a reproduction of the exact results reported in the reference research paper.

The current model is evaluated on the eight sensor nodes represented in the dataset. Generalisation to unseen nodes requires further investigation.

## Author

**Anushka**

B.Tech – Electronics and Computer Engineering  
Thapar Institute of Engineering and Technology

## Acknowledgements

Thanks to the authors of the LoRaWAN dataset and the reference research paper for making this work possible.
