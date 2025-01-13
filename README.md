# California Housing Price Prediction using Batch Gradient Descent

This project demonstrates the process of predicting California housing prices using the California Housing dataset. The dataset is processed, cleaned, and then used to train a custom Batch Gradient Descent model for regression. The project implements K-Fold Cross-Validation to evaluate the model's performance.

---

## Table of Contents
- [Dataset](#dataset)
- [Features](#features)
- [Project Workflow](#project-workflow)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Visualization](#visualization)
- [Results](#results)
- [License](#license)

---

## Dataset
The project uses the [California Housing Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html) available in scikit-learn. This dataset contains 8 numerical features and a target variable (`MedHouseVal`) that represents the median house value for California districts.

---

## Features
### Input Features:
- `MedInc`: Median income in block group
- `HouseAge`: Median house age in block group
- `AveRooms`: Average rooms per household
- `AveBedrms`: Average bedrooms per household
- `Population`: Block group population
- `AveOccup`: Average household size
- `Latitude`: Block group latitude
- `Longitude`: Block group longitude

### Target:
- `MedHouseVal`: Median house value (in $100,000s)

---

## Project Workflow
1. **Data Preprocessing**:
   - Load the dataset.
   - Handle missing values (if any).
   - Remove multicollinear features using a correlation threshold.
   - Remove outliers using the Interquartile Range (IQR) method.

2. **Feature Scaling**:
   - Standardize the features using `StandardScaler`.

3. **Model Training**:
   - Implement Batch Gradient Descent for linear regression.
   - Train the model using K-Fold Cross-Validation.

4. **Evaluation**:
   - Evaluate the model using R² score.
   - Track training and validation losses during the training process.

5. **Visualization**:
   - Plot the mean training and validation losses across epochs.

---

## Requirements
This project requires the following Python libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tqdm`

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ayushjoshi181999/California-Housing-Price-Prediction-using-Batch-Gradient-Descent.git
   cd California-Housing-Price-Prediction-using-Batch-Gradient-Descent
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Python notebook.

---

## Usage
The script performs the following steps:
1. Loads and preprocesses the California Housing dataset.
2. Removes multicollinear features and outliers.
3. Trains the regression model using Batch Gradient Descent with K-Fold Cross-Validation.
4. Outputs evaluation metrics (R² score) and visualizes the training and validation losses.

---

## Visualization
The script generates a plot showing:
- Mean training loss across epochs.
- Mean validation loss across epochs.

---

## Results
- **Average R² Score:** <Insert results after running the script>
- **Training and Validation Loss:** See the generated plot.

---

