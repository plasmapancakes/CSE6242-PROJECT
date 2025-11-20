# README.txt

## DESCRIPTION

This package contains the full implementation for **Team 037 — NFL Spread Prediction using Data-Driven Modeling and Interactive Visualization** for CSE 6242.
The project builds an end-to-end pipeline that predicts whether the home team will cover the point spread in an NFL game, using pregame-only, leakage-free features.

The system integrates:

1. Data Pipeline – loads historical team stats, betting lines, weather, rest, and situational features.
2. Feature Engineering – constructs pregame-only features, removes leakage, aligns metadata, and builds multiple feature sets.
3. Custom Objective Function – optimizes predictive accuracy, disagreement accuracy, disagreement frequency, and expected value.
4. Model Training – trains an XGBoost model using chronological splits, threshold sweeps, and weight grid search.
5. Evaluation Framework – computes calibration curves, per-week results, EV analysis, leakage tests, feature importance, and full predictions.
6. Interactive Dashboard – displays per-game predictions, feature-set comparisons, calibration plots, feature importance, weight sweep results, and 2025 predictions.

Execution time: **30–60 minutes**.

## INSTALLATION

### Python Version
Python 3.10 or later.

### Install Dependencies
Run:

    pip install -r requirements.txt

Required packages are listed in `requirements.txt`.

## EXECUTION

To run the full system:

1. Launch Jupyter:
       jupyter lab
   or
       jupyter notebook

2. Open:
       CSE6242 PROJECT.ipynb

3. Click:
       Run → Run All

Runtime: 30–60 minutes.

The notebook produces all dataframes, tables, metrics, plots, and dashboard components automatically. You are able to interact with the dashboards directly inside jupyter notebook. Please note that it will download a weather cache for all relevant weather information. This data can be quite large. 


##