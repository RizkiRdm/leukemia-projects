# Project 2: Leukemia Risk Factor Analysis - Data Preparation

**Notebook Objectives:**

* Preparing data for risk factor analysis.
* Loading dataset (reuse from Project 1).
* Data cleaning (handling low BMI anomalies? - according to strategy chosen).
* Feature selection (select relevant columns for risk factor analysis).
* Data transformation (if needed).
* Data splitting (if required for validation of prediction model in Project 2).

**Outline Notebook:**

1.  **Setup Environment & Import Libraries:**
    * Import pandas, numpy, scipy.stats, statsmodels, matplotlib, seaborn, etc.
    * Setting the visualization style (seaborn style).

2.  **Load Dataset:**
    * Load leukemia dataset (e.g. `leukemia_dataset.csv` from `data/project_1_descriptive_analysis/data/` folder).

3.  **Data Cleaning (Continued):**
    * [Low BMI anomaly handling strategy - describe the chosen strategy and implement the code].

4.  **Feature Selection:**
    * Select columns that will be analyzed as potential risk factors (based on Project 1 insights).
    * For example: `Smoking_Status`, `Family_History`, `Genetic_Mutation`, `WBC_Count`, `Bone_Marrow_Blasts`, etc.

5.  **Data Transformation (If Required):**
    * [Data transformation steps if required - e.g. encoding ordinal category columns, scaling numeric data, etc.].

6.  **Data Splitting (If Required for Prediction Model):**
    * [Splitting data into training set and test set if Project 2 includes a leukemia risk prediction model].

7.  **Save Prepared Data (Optional):**
    * [Save the prepared data to a new file (e.g. `leukemia_prepared_data.csv` in the `data/project_2_risk_factor_analysis/data/` folder) if you want to split from the analysis notebook].

**Next Notebooks Project 2:**

* `02_hypothesis_testing.ipynb`: Notebook for group comparison hypothesis testing (Chi-Square, T-test/Mann-Whitney U).
* `03_regression_analysis.ipynb`: Notebook for logistic regression analysis.
* `04_model_evaluation.ipynb` (Optional): Notebook for prediction model evaluation (if there is a prediction model in Project 2).

Translated with DeepL.com (free version)