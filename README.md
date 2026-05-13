# Loan Approval Prediction Analysis

**Anna Luu & Brenden Barry** - University of California, Davis

## Description

This project develops and evaluates machine learning models for predicting loan approval outcomes based on borrower financial profiles. Using a 50,000-sample dataset sourced from Kaggle, we benchmarked three classification approaches such as Logistic Regression, Random Forest, and Gradient Boosting. We set a target of achieving 90%+ accuracy. Through iterative refinement, including feature scaling and feature engineering, our best model (Gradient Boosting) achieved **92.04% accuracy** with an **AUC of 0.980**.

## Getting Started

### Dataset

Download the dataset from Kaggle using the link below and save it as a `.csv` file:

🔗 **[Realistic Loan Approval Dataset | US & Canada](https://www.kaggle.com/datasets/parthpatel2130/realistic-loan-approval-dataset-us-and-canada?resource=download)**

\*The CSV is also available directly in this repo

**Dataset license:** [Creative Commons BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

### Running the Code

The primary notebook is **"FinalDraft"**, which contains the full model. Open it in Google Colab, then load the dataset using one of the following methods:

1) Upload the CSV file directly when prompted in the notebook.

2) Save the CSV to your Google Drive, then mount your Drive within Colab to access it.

Once the dataset is loaded, run all cells to reproduce the results.

## Results

0) Model -> Accuracy
1) Logistic Regression (numeric features only) -> 73.56%
2) Logistic Regression (+ categorical features) -> 73.89%
3) Logistic Regression (+ StandardScaler) -> 87.08%
4) Random Forest -> 91.41%
5) **Gradient Boosting** -> **92.04%**
6) Feature Engineering models -> insignificant

The 90% accuracy target was met by both Random Forest and Gradient Boosting. "credit_score" was the top predictive feature in both models.
 
## Tech Stack
 
- **Language:** Python (.ipynb)
- **Libraries:** scikit-learn, pandas, NumPy, matplotlib, seaborn
- **Environment:** Google Colab
