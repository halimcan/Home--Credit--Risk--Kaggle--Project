 Home Credit Default Risk – Kaggle Project
 
Project Overview

This project focuses on credit default risk prediction using the Home Credit dataset from Kaggle.
The goal is to build a robust, reproducible machine learning pipeline that predicts the probability of loan default based on historical applicant data.

The project emphasizes:

Clean data preprocessing

Feature engineering

Model training & evaluation

Reproducibility and scalability


Project Structure

home-credit-risk/

├── data
    ├── raw    
    ├── processed
    
├── notebooks/

│   ├── 01_eda.ipynb

│   ├── 02_feature_engineering.ipynb

│   └── 03_modeling.ipynb

├── outputs/reports
    ├── FINAL_MODEL_Report 
    
├── requirements.txt

├── readme.md

└── .gitignore


Dataset

Due to size limitations, raw and processed datasets are not included in this repository.

Data Source

Kaggle – Home Credit Default Risk

https://www.kaggle.com/competitions/home-credit-default-risk

Expected Data Structure

After downloading, place the data under:

data/
├── raw/
│   ├── application_train.csv
│   ├── application_test.csv
│   ├── bureau.csv
│   └── previous_application.csv
└── processed/


All notebooks and scripts assume this folder structure.


Environment Setup
1️) Create virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate

2️) Install dependencies
pip install -r requirements.txt

* How to Run

Download the dataset from Kaggle

Place files under data/raw/

Run notebooks in order:

01_eda.ipynb
02_feature_engineering.ipynb
03_modeling.ipynb


Modeling Approach

Handling missing values

Feature engineering across multiple tables

Train / validation split

Model evaluation using appropriate classification metrics

The focus is on interpretable and reproducible results, not leaderboard overfitting.


Evaluation Metrics

ROC-AUC
KS Score


(Details and results are available inside the modeling notebook.)


Key Learnings

Working with large, multi-table financial datasets

Designing a clean ML pipeline

Preventing data leakage

Managing large datasets outside GitHub


Notes

Notebook outputs are intentionally cleared before commits.

Large datasets are excluded via .gitignore.

The repository is designed to be lightweight and reviewer-friendly.





