# PySpark Income Prediction (UCI Adult Dataset)

## Overview
This project builds an end-to-end machine learning pipeline in PySpark to predict whether a person earns >50K/year using the UCI Adult dataset. It demonstrates big data preprocessing, feature engineering, and model training at scale.

## Dataset
- UCI Adult Income dataset (loaded directly from the UCI repository URL)
- Target: income (<=50K vs >50K)

## Workflow
- Load data into Spark
- Clean and preprocess (trim values, handle missing “?”)
- Cast numeric features
- Encode categorical features (StringIndexer + OneHotEncoder)
- Assemble features with VectorAssembler
- Train and evaluate:
  - Logistic Regression
  - Gradient-Boosted Trees (GBTClassifier)

## Tech Stack
- PySpark (Spark ML)
- Python
- Pandas (initial loading)

## How to Run
1. Install Apache Spark (or use Databricks / local Spark).
2. Install Python dependencies:
   pip install pyspark pandas
3. Open and run:
- `pyspark_income_prediction.ipynb`

## Results
Model performance is evaluated using Spark ML evaluators (e.g., accuracy/ROC depending on the notebook configuration).
