![image](https://github.com/user-attachments/assets/45ec226c-888a-4ae3-bfd1-c6382cb580b8)
# Credit Risk Modeling Project

## Overview
This project involves building a credit risk classification model to predict the approval status of loan applicants. The model is based on demographic and financial features of applicants. Various machine learning models, including Random Forest, XGBoost, and Decision Trees, are used to achieve optimal prediction performance. The project also involves feature engineering, statistical testing, and model evaluation.

## Dataset
The dataset includes the following key columns:
- **PROSPECTID**: Unique identifier for each applicant
- **Total_TL**: Total number of trade lines
- **Tot_Closed_TL**: Number of closed trade lines
- **Tot_Active_TL**: Number of active trade lines
- **pct_active_tl**: Percentage of active trade lines
- **pct_closed_tl**: Percentage of closed trade lines
- **Auto_TL**: Auto trade lines
- **PL_TL**: Personal loan trade lines
- **Age_Oldest_TL**: Age of the oldest trade line
- **Approved_Flag**: Target variable indicating loan approval status

## Key Features
- **Chi-square tests** for feature selection of categorical variables.
- **ANOVA tests** for selecting significant numerical variables.
- **Variance Inflation Factor (VIF)** analysis to remove multicollinear features (VIF < 6).
- **Sentiment Analysis** for determining the potential risk of default based on financial behavior.

## Prerequisites
- Python 3.6+
- Required Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scikit-learn`
  - `statsmodels`
  - `xgboost`

Install the required libraries using:

```bash
pip install numpy pandas matplotlib scikit-learn statsmodels xgboost
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/credit-risk-modeling.git
cd credit-risk-modeling
Place the dataset files (case_study1.xlsx, case_study2.xlsx) in the project directory.

Run the following command to preprocess the data and train the models:

bash
Copy code
python credit_risk_modeling.py
Usage
Once the models are trained, you can:

Predict loan approval status.
Evaluate model performance using metrics like accuracy, precision, recall, and F1 score.
Modeling Approach
Data Cleaning: Placeholder values (-99999) were removed, and null values were handled.
Feature Selection: Chi-square tests for categorical features and ANOVA tests for numerical features. Multicollinearity was reduced using VIF analysis.
Modeling:
Random Forest: Achieved 85.4% accuracy.
XGBoost: Achieved the best accuracy of 87.3%.
Decision Tree: Achieved 81.6% accuracy.
Evaluation: Models were evaluated using precision, recall, and F1 score.
Results
XGBoost achieved the best performance with an accuracy of 87.3% and a precision of 0.91 for high-risk class (P1).


credit modelling
==============================




this is about credit modelling project

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
