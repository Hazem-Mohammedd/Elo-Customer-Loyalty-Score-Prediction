# Elo-Customer-Loyalty-Score-Prediction
This project applies various machine learning techniques to predict customer loyalty scores for Elo, one of the largest payment brands in Brazil. The aim is to help Elo target more loyal customers for offers and promotions, optimizing marketing campaigns and reducing waste.

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Solution Approach](#solution-approach)
- [Data Sources & Overview](#data-sources--overview)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Team Members](#team-members)
- [Acknowledgements](#acknowledgements)

---

## Project Overview
This project analyzes customer loyalty using data from the Elo Merchant Category Recommendation Kaggle competition. The aim is to predict loyalty scores for cardholders, so Elo can recommend relevant merchant promotions, enhance customer satisfaction, and minimize unwanted marketing campaigns.

---

## Problem Statement
Payment brands use partnerships with merchants to offer special promotions/discounts to cardholders. However, these promotions are not always sufficiently personalized, and many campaigns reach customers who are unlikely to respond. Assigning a loyalty score to each cardholder enables Elo to target only those who are most likely to utilize these offers, optimizing engagement and reducing waste.

---

## Solution Approach
**Formulation:** Regression problem, where the target is the loyalty score.

**Workflow:**
- Data preprocessing and quality assessment
- Exploratory data analysis and visualization
- Feature engineering and aggregation
- Training and evaluation of regression models (Linear Regression, XGBoost, CatBoost, LightGBM, etc.)
- Model selection based on RMSE and R²

**Evaluation Metrics:**
- RMSE (Root Mean Squared Error)
- R-squared (Coefficient of Determination)

---

## Data Sources & Overview

**Data Origin:** [Kaggle Elo Merchant Category Recommendation](https://www.kaggle.com/c/elo-merchant-category-recommendation/data)

**Files:**
- `train.csv` & `test.csv`: Card IDs, card info, and (in train.csv) true loyalty scores.
- `historical_transactions.csv`: Up to 3 months’ transactions per card.
- `new_merchant_transactions.csv`: Two months of transactions with new merchants (that the card had not visited before).
- `merchants.csv`: Aggregated merchant info.
- `Data_Dictionary.xlsx`: Descriptions of all data fields.

**Note:** Due to the large size of the transaction files, a dedicated notebook was created specifically for processing and analyzing the transactions data. All other processing and analysis steps for the remaining files, as well as all modeling and evaluation, are performed in a separate notebook.

---

## Technologies Used
- **Programming & Libraries:** Python, Numpy, Pandas, Scikit-learn, Matplotlib, Seaborn, LightGBM, XGBoost, CatBoost.
- **Modeling Approaches:** Regression algorithms (Linear Regression, Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting, AdaBoost, LightGBM, XGBoost, KNN, CatBoost).
- **Version Control & Collaboration:** Git, GitHub Projects.

---
  
## 6. Helper Functions
To keep the code organized and reusable, a separate Python script (`Helpers.py`) contains helper functions for data preparation, and exploratory data analysis. This keeps the notebooks clean and makes the project easier to maintain.

---

## How to Run

1. Clone the repository to your computer.
2. Set up a Python environment.
3. Download the dataset from Kaggle and place files in the project directory.
4. Install dependencies such as numpy, pandas, scikit-learn, matplotlib, seaborn, and others.
5. Handle large files: The dataset includes large CSV files (e.g., historical_transactions.csv ~2.8 GB). You can download all data from the link in the data source section.

---

## Team Members

- Hazem Mohamed Samy – hazemmuhammedd1@gmail.com
- Mahmoud Emam Elhout – ma7moudel7out@gmail.com
- Tarek Ahmed Ali – Tareahme@gmail.com
- Asmaa Gamal AbdElnasser – gasmaa188@outlook.com

---

## Acknowledgements

- [Kaggle Elo Merchant Competition](https://www.kaggle.com/c/elo-merchant-category-recommendation)
- Open source libraries: scikit-learn, pandas, XGBoost, CatBoost, LightGBM, seaborn, matplotlib, etc.
