# Child Mortality Analysis — Cross-Sectional Regression Using WDI

This repository contains a machine learning project on under-five mortality using World Development Indicators (WDI).

## Project objective

The project predicts and explains cross-country differences in under-five mortality in 2023 using lagged WDI indicators. The final modeling dataset is cross-sectional: each country appears once.

## Students

- Ayoub Taychi
- Hajar Lasri
- Yama Saputra

## Main notebook

Use this notebook to reproduce the complete project from start to finish:

`notebooks/child_mortality_wdi_cross_sectional_regression.ipynb`

The split stage notebooks are included for reading and GitHub organization. Some later stage notebooks depend on variables created in previous stages, so the full notebook is the safest one to run.

## How to run

1. Place the raw CSV file in the same folder as the main notebook or in the project root:
   `WB_WDI_WIDEF (1).csv`
2. Open `notebooks/child_mortality_wdi_cross_sectional_regression.ipynb`.
3. Run all cells from top to bottom.
4. The notebook generates a `results/` folder with data, tables, visualisations, models, and report outputs.

## Methodology summary

- Task type: regression
- Target: under-five mortality rate in 2023
- Final data structure: one row per country
- Predictors: information before 2023 only
- Historical information: 2022 levels, 2018–2022 means, and 2018–2022 changes
- Feature selection: train-only screening, leakage filtering, redundancy reduction
- Models: Dummy baseline, Ridge, ElasticNet, KNN, Random Forest, Extra Trees, Gradient Boosting, and optional XGBoost
- Evaluation: cross-validation on training data and final evaluation on the held-out test set

## Folder guide

- `notebooks/` contains the full notebook and stage-split notebooks.
- `results/` is generated when the notebook runs.
- Raw data is not included unless you decide to upload it.

## Stage files

1. `01_stage_1_problem_definition.ipynb` — research question and project design
2. `02_stage_2_data_collection.ipynb` — raw data loading and structure audit
3. `03_stage_3_data_cleaning_preprocessing.ipynb` — cleaning, countries, target definition
4. `04_stage_4_exploratory_data_analysis.ipynb` — EDA and visualisations
5. `05_stage_5_feature_pool_construction.ipynb` — leakage-safe feature pools
6. `06_stage_6_data_splitting.ipynb` — country-level train/test split
7. `07_stage_7_feature_selection_final_dataset.ipynb` — train-only feature selection and final dataset
8. `08_stage_8_model_selection.ipynb` — model setup
9. `09_stage_9_model_training_cross_validation.ipynb` — training and cross-validation
10. `10_stage_10_evaluation_tuning_interpretation.ipynb` — tuning, evaluation, feature importance, robustness
11. `11_stage_11_12_deployment_monitoring_conclusion.ipynb` — deployment discussion, monitoring, conclusion
