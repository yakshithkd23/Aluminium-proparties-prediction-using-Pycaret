# Alrodynamics
# Aluminum Rod Properties Prediction

This project focuses on predicting key mechanical and electrical properties of aluminum rods, such as Ultimate Tensile Strength (UTS), Elongation, and Conductivity (%IACS), using machine learning models. The dataset contains various features related to material properties, and the goal is to build accurate predictive models using both Neural Networks and Random Forests.

## Project Overview

### Objective
The objective of this project is to predict the following properties of aluminum rods:
- **Ultimate Tensile Strength (UTS)** in MPa
- **Elongation** as a percentage (%)
- **Conductivity** as a percentage of International Annealed Copper Standard (%IACS)

### Dataset
The dataset consists of various features related to the material and mechanical properties of aluminum rods. The target variables include:
- UTS (MPa)
- Elongation (%)
- Conductivity (%IACS)

The features are scaled to improve the performance of the machine learning models.

### Models Used
1. **Neural Networks**: A deep neural network built using Keras, consisting of multiple hidden layers with `tanh` activations. The model is trained for 200 epochs.
2. **Random Forest Regressors**: A powerful ensemble method used for regression tasks. It serves as a baseline for comparison with the neural network.

### Model Evaluation
The performance of each model is evaluated using:
- **R² (Coefficient of Determination)**
- **Mean Absolute Error (MAE)**

Graphical visualizations of the predictions compared to the true values are also provided.

### PyCaret Integration
This project leverages **PyCaret**, an automated machine learning (AutoML) library, to streamline the process of model comparison and selection. PyCaret compares different regression models and helps select the best-performing model for each property (UTS, Elongation, and Conductivity).

## Key Features
- **Data Visualization**: A heatmap is provided to analyze correlations between features.
- **Model Comparison**: PyCaret is used to automatically compare and select the best models.
- **Prediction and Evaluation**: Both neural networks and random forests are used to predict UTS, Elongation, and Conductivity, and the performance is evaluated.
- **Graphical Output**: Scatter plots visualize how well the model predictions match the actual values.

## Installation
To run this project, you need to install the required libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn keras pycaret
