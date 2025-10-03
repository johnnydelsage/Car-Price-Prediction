# Car Price Prediction

Machine learning project for predicting used car prices based on technical specifications and market data. The goal is to build and compare several regression models and achieve RMSE < 2500.

## Project Description
Cars can have very different prices depending on mileage, age, engine power, brand, and other parameters. This project demonstrates how ML models can be applied to predict car prices and help buyers or sellers estimate the fair market value.

Workflow:
1. Data preprocessing – cleaning, handling categorical and numerical features, scaling & encoding with ColumnTransformer.
2. Model training – testing multiple regressors:
   - Linear Regression & Ridge
   - Decision Tree & Random Forest
   - LightGBM (gradient boosting)
3. Hyperparameter tuning with GridSearchCV inside Pipeline (no data leakage).
4. Model evaluation – comparing performance with RMSE metric, analyzing training and prediction time.

## Tech Stack
- Python 3.13
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- LightGBM

## Results
- Best performing model: LightGBM
- Achieved RMSE < 2500 (target reached)
- Compared training time vs prediction speed across models

## How to Run
Clone the repo:
git clone https://github.com/artemxdata/Car-Price-Prediction.git
cd car-price-prediction


## Create and activate a virtual environment:
- python -m venv venv
- source venv/bin/activate # Linux/Mac
- venv\Scripts\activate # Windows


## Install dependencies:
pip install -r requirements.txt


## Run Jupyter Notebook:
jupyter notebook "Car Price Prediction.ipynb"


## Project Structure
├── .gitignore # Git ignore file
├── autos.csv # Dataset with car information
├── Car Price Prediction.ipynb # Main notebook with full ML pipeline
├── LICENSE # Project license
├── README.md # Project description and instructions
└── requirements.txt # Minimal dependencies


## Future Improvements
- Add more feature engineering (engine volume, region, condition, etc.)
- Try additional boosting models (XGBoost, CatBoost)
- Deploy as a simple web app for interactive car valuation

## Author
Made for educational and practical purposes.


