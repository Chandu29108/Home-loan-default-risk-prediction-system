# 🏦 Home Loan Default Risk Prediction System 🚀

> **Tagline:** Predict loan defaults with ~78% AUC using Home Credit risk data.
> 
## Dataset :

Link : (https://www.kaggle.com/c/home-credit-default-risk/data)

## Table of Contents

* Overview
* Repository Structure
* Features
* Demo
* Installation
* Usage
* Results
* Models
* Challenges
* Contributing
* Business case
* Future Enhancements
* License

## Overview

**Home Loan Default Prediction – Risk Management System**

This project performs an **end-to-end data science pipeline** for predicting whether a borrower will default on a home loan. The workflow includes:

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Training multiple machine learning models
* Hyperparameter tuning
* Model evaluation using business-relevant metrics
* Saving the best model for future deployment

**Business Goal:**
Help banks and financial institutions reduce credit risk by identifying high-risk applicants early in the loan approval process.

## Repository Structure

Home-loan-default-risk-prediction-system/
│
├── Home Loan Default Prediction-Risk Management.ipynb   # Main notebook
├── models/                                              # Saved ML models
│   └── *.pkl files / *.csv
├── results/                                             # Outputs, plots, and metrics
│   └── *.png 
├── requirements.txt                                     # Python dependencies
└── LICENSE                                              # MIT License

## Features

* Loads **7 CSV datasets** (≈ 300,000+ loan applications)
* Handles missing values and class imbalance
* Advanced EDA:

  * Distribution plots
  * Correlation analysis
  * Missing value heatmaps
* Feature engineering from:

  * Bureau data
  * Previous applications
  * Payment history
* Trains multiple ML models with cross-validation
* Evaluates using:

  * ROC-AUC
  * F1-score
  * Precision–Recall curves

## 🎬 Demo

Run the notebook for interactive visualizations:

[Open in Colab](https://colab.research.google.com/drive/1S0lOAbwpZ2h4JQ7dAkMH7RlcPSFKAdx7)

## Installation

git clone https://github.com/Chandu29108/Home-loan-default-risk-prediction-system.git
cd Home-loan-default-risk-prediction-system
pip install -r requirements.txt

## Usage

Open the main notebook:

Home Loan Default Prediction-Risk Management.ipynb

Run all cells sequentially in:

* Jupyter Notebook or
* Google Colab

Outputs (models & results) will be saved in:


/models/
/results/

## 🤖 Models Used

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost
* LightGBM (Final Model with Bayesian Optimization)

## Results

Best performing models:

| Model                | ROC-AUC     |
| -------------------- | ----------- |
| Logistic Regression  | 0.58        |
| Decision Tree        | 0.58        |
| Random Forest        | 0.75        |
| **XGBoost**          | **0.76**    |
| **LightGBM (Tuned)** | **0.781** ✅ |

Final predictions saved as:

results/final_predictions_test.csv

Columns include:

* `SK_ID_CURR`
* `TARGET_actual`
* `TARGET_pred` (default probability)

## Challenges

* Severe class imbalance (few defaulters)
* Large dataset with multiple related tables
* High dimensional feature space
* Choosing the right trade-off between precision and recall
* Computational cost of hyperparameter tuning

---

## Contributing

Contributions are welcome! You can:

* Fork the repo
* Create a new branch
* Add improvements
* Submit a pull request

##  Business Use Case

This system can be used by:

* Banks
* NBFCs
* Credit Rating Agencies
* FinTech Companies

To:

* Reduce bad loans
* Improve risk assessment
* Automate credit decisions
* 
##  Future Enhancements

Planned improvements:

1. Deploy as a Flask / FastAPI web app
2. Build Streamlit dashboard
3. Integrate with real-time loan systems
4. Add explainable AI (SHAP values)
5. Monitor model drift in production
   
## License

This project is licensed under the **MIT License** — see the LICENSE file for details.

---

## 👤 Author

**Chandu Vanja**
B.Tech (ECE), NIT Durgapur
Machine Learning & Data Science Enthusiast

📧 mailto:vc21u10786@gmail.com
🔗 GitHub: Chandu29108


