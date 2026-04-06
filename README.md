# Car Price Prediction ML Project
## Overview
This repository contains a Machine Learning project to predict car-related features based on an existing dataset (`car_price_prediction.csv`). The project covers a complete end-to-end machine learning pipeline, starting from data ingestion all the way through to model evaluation.

## Project Structure
- `Car_predication.ipynb`: A Jupyter Notebook containing the code and detailed steps for the machine learning pipeline.
- `car_price_prediction.csv`: The dataset containing information about various cars, such as Price, Manufacturer, Model, Production Year, Category, Leather interior, Fuel type, Engine volume, Mileage, Cylinders, Gear box type, Drive wheels, Doors, Wheel, Color, and Airbags.

## Workflow Pipeline
The notebook is structured into the following sequential steps:
1. **Dataset Load**: Importing the dataset using Pandas to explore the initial raw data.
2. **Data Visualization**: Analyzing the data distributions and discovering patterns using visualizations (e.g., plotting the top 10 manufacturers, distribution of gearbox types).
3. **Data Pre-processing**: Cleaning the dataset, dropping redundant columns, and resolving outliers/missing values.
4. **Data Divide (X, y)**: Isolating the descriptive features (X) from the designated target variable (y).
5. **Encoding & Scaling**:
   - Transforming categorical variables into numerical values utilizing `LabelEncoder`.
   - Scaling continuous numerical features using `StandardScaler`.
   - Performing feature selection using `SelectKBest` algorithms alongside `chi2`.
6. **Splitting**: Dividing the dataset into randomized training and test sets via `train_test_split`.
7. **Model Implementation**: Implementing multiple classification models natively, including:
   - K-Nearest Neighbors (KNN) Classifier
   - Decision Tree Classifier
8. **Evaluation**: Assessing model accuracy and effectiveness using metrics like `accuracy_score`, `classification_report`, and `confusion_matrix`.

## Requirements
To run this notebook, the following Python dependencies must be installed:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

You can easily install them via pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run
1. Clone or download this repository to your local machine.
2. Ensure the `car_price_prediction.csv` dataset is present in the same directory as the notebook.
3. Open a terminal or command prompt and launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open the `Car_predication.ipynb` file from the Jupyter dashboard.
5. Execute the notebook cells sequentially to walk through the EDA, data preparation, and machine learning models.
