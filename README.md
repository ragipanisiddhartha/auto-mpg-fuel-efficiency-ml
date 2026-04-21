# Predicting Vehicle Fuel Efficiency Using Machine Learning

MSc Data Science Final Project Report  
University of Hertfordshire

## Project overview

This project investigates how accurately vehicle fuel efficiency, measured in miles per gallon (mpg), can be predicted from technical vehicle attributes using supervised machine learning. The analysis is based on the Auto MPG dataset from the UCI Machine Learning Repository.

The project compares five regression models:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor

The aim is to identify which model gives the best predictive performance and to understand which vehicle features contribute most strongly to fuel efficiency.

## Research question

How accurately can fuel efficiency (mpg) be predicted from vehicle attributes such as cylinders, displacement, horsepower, weight, acceleration, model year and origin, and which regression model provides the best predictive performance on the Auto MPG dataset?

## Dataset

- Source: UCI Machine Learning Repository
- Dataset: Auto MPG
- Original records: 398
- Final cleaned records: 392

The dataset includes:

- mpg
- cylinders
- displacement
- horsepower
- weight
- acceleration
- model_year
- origin
- car_name

The target variable is `mpg`.

## Methodology

The workflow used in this project is:

1. Load the raw Auto MPG dataset
2. Clean missing horsepower values and remove incomplete rows
3. Perform exploratory data analysis
4. Select numeric features for modelling
5. Split the data into training and test sets (80/20)
6. Train and evaluate models using 5-fold cross-validation
7. Tune hyperparameters using GridSearchCV
8. Compare models using RMSE, MSE and R²
9. Interpret the final Random Forest model using feature importance

## Main results

The Random Forest Regressor achieved the best overall performance.

### Test set performance

| Model | Test RMSE | Test R² |
|---|---:|---:|
| Linear Regression | 3.10 | 0.84 |
| Ridge Regression | 3.12 | 0.84 |
| Lasso Regression | 3.15 | 0.83 |
| Decision Tree | 3.90 | 0.75 |
| Random Forest | 2.29 | 0.91 |

## Key findings

- Random Forest produced the lowest prediction error and highest R².
- Weight and displacement were the most important predictors.
- Horsepower and model year also contributed strongly.
- Linear models performed reasonably well, but could not capture non-linear structure as effectively as Random Forest.

## Repository structure

```text
auto-mpg-fuel-efficiency-ml/
│
├── README.md
├── requirements.txt
│
├── notebooks/
│   └── Siddhartha_24074708.ipynb
│
└── reports/
    ├── (Report)Siddhartha_24074708.pdf
    └── Predicting Automobile Fuel Efficiency Using Machine Learning.pdf
```

## Files

- `notebooks/Siddhartha_24074708.ipynb` — Jupyter notebook containing the full data cleaning, exploratory data analysis, model training, evaluation, and visualisations.
- `reports/Siddhartha_24074708.pdf` — Final MSc project report.
- `reports/Predicting Automobile Fuel Efficiency Using Machine Learning.pdf` — Project presentation slides in PDF format.
- `requirements.txt` — Python dependencies required to run the notebook.



## How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/ragipanisiddhartha/auto-mpg-fuel-efficiency-ml.git
   ```

2. Move into the project folder:
   ```bash
   cd auto-mpg-fuel-efficiency-ml
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook:
   ```bash
   jupyter notebook
   ```

## Requirements

Typical Python libraries used:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

## Report

The final MSc project report is included in the repository/report folder.

## Author

Siddhartha Ragipani  
MSc Data Science  
University of Hertfordshire

## Supervisor

Sunina Sharvy

## License

This repository is for academic submission and educational purposes.

