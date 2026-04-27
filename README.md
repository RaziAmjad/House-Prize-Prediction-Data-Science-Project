Leader Razi Amjad 176

Contributed By

Eman Fazal 181
Fatima Zaffar 165
Falak Shehzad 163
Sajal Shehwar 192
Muaz Asif 184


House Price Prediction

A machine learning project that predicts Boston house prices using a Random Forest model.

 Project Structure

House Prize Prediction/
├── boston.csv                        # Dataset

├── boston_house_price_prediction.ipynb  # Main notebook

├── data_split.pkl                    # Saved train/test split

├── model.pkl                         # Trained model

├── result.png                        # Actual vs Predicted plot

└── house_price_project/
    └── venv/                         # Python virtual environment

 Dataset

**Boston Housing Dataset** — 506 rows, 14 columns. Target variable: `MEDV` (median house value in $1000s).

Key features include crime rate, number of rooms, distance to employment centers, tax rate, and more.

Pipeline

The notebook is split into 4 scripts:

1. **preprocess.py** — Loads `boston.csv`, splits into 80/20 train-test, saves to `data_split.pkl`
2. **train_model.py** — Trains a `RandomForestRegressor` (100 trees), saves to `model.pkl`
3. **evaluate.py** — Calculates MSE, RMSE, R² and saves an Actual vs Predicted scatter plot as `result.png`
4. **predict.py** — Loads the model and predicts the price of a single sample house

 How to Run

bash
1. Activate virtual environment
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux

 2. Install dependencies (if needed)
pip install pandas scikit-learn matplotlib

 3. Run the notebook cells in order, or run scripts individually
python preprocess.py
python train_model.py
python evaluate.py
python predict.py
```

 Output

- **result.png** — Scatter plot comparing actual vs predicted prices
- **model.pkl** — Saved trained model (reusable without retraining)
- Console prints MSE, RMSE, and R² score after evaluation

Requirements

- Python 3.x
- pandas
- scikit-learn
- matplotlib
