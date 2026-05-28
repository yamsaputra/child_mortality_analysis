

This folder contains the project notebook split by workflow stage.

## Important note

The code cells were **not rewritten or modified**. The original notebook was only split into smaller notebooks by stage for easier GitHub organization.

The complete original notebook is also included:

- `notebooks/00_full_project_original.ipynb`

If you want to run the entire project from start to finish, use the full original notebook. The split notebooks are mainly for reading, reviewing, and presenting the project stage by stage because later stages depend on variables created in earlier stages.

## Run / reading order

1. `01_stage_1_problem_definition.ipynb`
2. `02_stage_2_data_collection.ipynb`
3. `03_stage_3_data_cleaning_preprocessing.ipynb`
4. `04_stage_4_eda.ipynb`
5. `05_stage_5_feature_pool_construction.ipynb`
6. `06_stage_6_data_splitting.ipynb`
7. `07_stage_7_feature_selection_final_dataset.ipynb`
8. `08_stage_8_9_model_selection_training.ipynb`
9. `09_stage_10_evaluation_tuning.ipynb`
10. `10_stage_11_12_discussion_conclusion.ipynb`

## Project design

- Task: regression
- Target: under-five mortality in 2023
- Final dataset: one row per country
- Predictors: 2022 values and 2018–2022 changes
- No classification
- No 2024 forecast as the main task
- Leakage-safe feature selection and model evaluation

## Manifest

| File | Section | Original cells | Cells | Code | Markdown |
|---|---|---:|---:|---:|---:|
| `notebooks/01_stage_1_problem_definition.ipynb` | Stage 1 — Problem Definition | 0–1 | 2 | 0 | 2 |
| `notebooks/02_stage_2_data_collection.ipynb` | Stage 2 — Data Collection | 2–20 | 19 | 9 | 10 |
| `notebooks/03_stage_3_data_cleaning_preprocessing.ipynb` | Stage 3 — Data Cleaning and Preprocessing | 21–38 | 18 | 8 | 10 |
| `notebooks/04_stage_4_eda.ipynb` | Stage 4 — Exploratory Data Analysis | 39–64 | 26 | 12 | 14 |
| `notebooks/05_stage_5_feature_pool_construction.ipynb` | Stage 5 — Leakage-Safe Feature Pool Construction | 65–71 | 7 | 3 | 4 |
| `notebooks/06_stage_6_data_splitting.ipynb` | Stage 6 — Data Splitting | 72–76 | 5 | 2 | 3 |
| `notebooks/07_stage_7_feature_selection_final_dataset.ipynb` | Stage 7 — Train-Only Feature Selection and Final Dataset Construction | 77–100 | 24 | 11 | 13 |
| `notebooks/08_stage_8_9_model_selection_training.ipynb` | Stage 8–9 — Model Selection, Training, and Cross-Validation | 101–110 | 10 | 4 | 6 |
| `notebooks/09_stage_10_evaluation_tuning.ipynb` | Stage 10 — Model Evaluation and Hyperparameter Tuning | 111–138 | 28 | 13 | 15 |
| `notebooks/10_stage_11_12_discussion_conclusion.ipynb` | Stage 11–12 — Deployment, Monitoring, and Final Conclusion | 139–141 | 3 | 0 | 3 |

C
