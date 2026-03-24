# Predicting Automobile Fuel Efficiency Using Machine Learning

MSc Data Science Individual Project – University of Hertfordshire  
Author: Siddhartha Ragipani (Student ID: 24074708)  
Supervisor: Sunina Sharvy  

This project uses the UCI Auto MPG dataset to build and compare regression
models that predict a car’s fuel efficiency (mpg) from basic technical
attributes such as cylinders, displacement, horsepower, weight, acceleration,
model year and origin. https://archive.ics.uci.edu/ml/machine-learning-databases/auto-mpg/auto-mpg.data

## Project goals

- Perform exploratory data analysis (EDA) on the Auto MPG dataset.
- Build baseline and advanced regression models (Linear, Ridge, Lasso,
  Decision Tree, Random Forest).
- Use cross-validation and hyperparameter tuning to optimise performance.
- Evaluate models using RMSE and R² on a held-out test set.
- Interpret the best-performing model and relate findings to the literature.

## Data

The dataset is the **Auto MPG** dataset from the UCI Machine Learning
Repository.(https://archive.ics.uci.edu/ml/machine-learning-databases/auto-mpg/auto-mpg.data)  
Original source: Dua, D. and Graff, C. (2019). UCI Machine Learning Repository.

You can download it from UCI and place it in the `data/` folder as
`auto-mpg.csv`, or adjust the paths in the notebooks accordingly.

## Environment

Create a conda environment:

```bash
conda create -n auto-mpg-ml python=3.11
conda activate auto-mpg-ml
pip install -r requirements.txt
