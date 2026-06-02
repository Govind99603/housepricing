# California Housing Price Prediction using Machine Learning

## Project Overview

This project builds a Machine Learning model to predict housing prices in California using the California Housing Dataset from Scikit-Learn. The project follows a complete ML workflow including data preprocessing, exploratory data analysis (EDA), feature scaling, model training, evaluation, and model serialization for future deployment.

The primary goal is to understand the relationship between housing features and property prices while implementing a complete regression-based machine learning pipeline.

---

## Problem Statement

Predict the median house value of California districts using demographic, geographic, and housing-related features.

This project uses Linear Regression to estimate housing prices based on various independent variables such as median income, house age, average rooms, population, and location-related information.

---

### Software and Tools Requirements

1. [Githun Account](https://github.com)
2. [VS Code IDE](https://code.visualstudio.com/)
3. [HerokuAccount](https://heroku.com)
4. [GitCLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)

---

Create a new environment

```
conda create -p venv python==3.13.9 -y
```
---

## Dataset Information

The dataset used is the California Housing Dataset provided by Scikit-Learn.

### Features

| Feature    | Description                   |
| ---------- | ----------------------------- |
| MedInc     | Median income in block group  |
| HouseAge   | Median house age              |
| AveRooms   | Average number of rooms       |
| AveBedrms  | Average number of bedrooms    |
| Population | Population of the block group |
| AveOccup   | Average occupancy             |
| Latitude   | Latitude coordinate           |
| Longitude  | Longitude coordinate          |

### Target Variable

| Target             |
| ------------------ |
| Median House Price |

---

## Project Workflow

### 1. Data Collection

* Loaded California Housing Dataset from Scikit-Learn.
* Converted the dataset into a Pandas DataFrame.
* Added the target variable (Price).

### 2. Data Exploration

* Dataset structure inspection
* Statistical summary generation
* Missing value analysis
* Correlation analysis

### 3. Data Cleaning

* Checked for missing values.
* Removed outliers using the Interquartile Range (IQR) method.

### 4. Exploratory Data Analysis (EDA)

Performed:

* Correlation analysis
* Pair plots
* Scatter plots
* Regression plots
* Feature-target relationship analysis

### 5. Feature Engineering

* Separated independent and dependent variables.
* Applied train-test split.
* Standardized features using StandardScaler.

### 6. Model Building

Implemented:

* Linear Regression

### 7. Model Evaluation

Evaluated model performance using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

### 8. Model Persistence

Saved:

* Feature scaler (`scaler.pkl`)
* Trained model (`regmodel.pkl`)

using Python Pickle for future deployment.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Pickle

---

## Project Structure

```bash
├── housepricing.ipynb
├── scaler.pkl
├── regmodel.pkl
├── README.md
```

---

## Machine Learning Pipeline

```text
Dataset
   ↓
Data Cleaning
   ↓
Outlier Removal
   ↓
EDA & Visualization
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Linear Regression Model
   ↓
Performance Evaluation
   ↓
Model Serialization
```

---

## Key Visualizations

The project includes:

* Correlation Analysis
* Pairplot Visualization
* House Age vs Price Analysis
* Median Income vs Price Analysis
* Regression Trend Plots
* Residual Distribution Plot
* Prediction vs Actual Plot

---

## Model Evaluation Metrics

| Metric   | Value                |
| -------- | -------------------- |
| MAE      | Update from notebook |
| MSE      | Update from notebook |
| RMSE     | Update from notebook |
| R² Score | Update from notebook |

---

## Sample Prediction

The trained model can predict house prices for unseen housing records after applying the same scaling transformation used during training.

Example workflow:

```python
scaled_data = scaler.transform(new_data)
prediction = model.predict(scaled_data)
```

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Data preprocessing
* Outlier detection and removal
* Exploratory Data Analysis (EDA)
* Feature scaling
* Linear Regression
* Model evaluation techniques
* Model serialization using Pickle
* End-to-end Machine Learning workflow

---

## Future Improvements

* Implement multiple regression algorithms.
* Perform hyperparameter tuning.
* Build a Streamlit web application.
* Deploy the model on cloud platforms.
* Add advanced feature engineering techniques.
* Compare ensemble learning models.

---

## Author

Developed as a Machine Learning project to understand regression modeling and housing price prediction using Python and Scikit-Learn.
