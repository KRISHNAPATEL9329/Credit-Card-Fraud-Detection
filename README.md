# Credit Card Fraud Detection using Machine Learning

**Student:** Madhu Jain  
**Programme:** Bachelor of Computer Applications (BCA)  
**Project area:** Data Analytics / Machine Learning

## Project description
This project demonstrates a machine-learning workflow for classifying credit-card transactions as legitimate (`Class = 0`) or potentially fraudulent (`Class = 1`). It explores class imbalance, preprocesses the data, trains Logistic Regression and Random Forest models, and compares fraud-class precision, recall, F1-score, and confusion matrices.

## Dataset
**Source:** [Credit Card Fraud Detection — Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

Download `creditcard.csv` from Kaggle and place it in the same folder as the notebook. The commonly distributed version has 284,807 rows and 30 columns, including `Time`, `Amount`, anonymized features `V1`–`V28`, and `Class`. Dataset access and use are subject to Kaggle's terms.

## Technologies used
- Python
- pandas and NumPy
- Matplotlib
- scikit-learn
- joblib
- Jupyter Notebook

## Project files
- `MadhuJain_CreditCardFraudDetection.ipynb` — code, analysis, training, and evaluation
- `requirements.txt` — Python dependencies
- `MadhuJain_ProjectReport.docx` — detailed report
- `README.md` — project overview and setup instructions

## Setup and execution
1. Install Python 3.10 or newer.
2. Download `creditcard.csv` from the dataset source above.
3. Put the CSV file beside the notebook.
4. (Recommended) Create and activate a virtual environment.
5. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

6. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

7. Open `MadhuJain_CreditCardFraudDetection.ipynb` and run all cells from top to bottom.

## Methodology
1. Load and inspect the dataset.
2. Explore class distribution and transaction amounts.
3. Split into train and test sets using stratification.
4. Standardize `Time` and `Amount` using a scaler fitted on training data only.
5. Train Logistic Regression and Random Forest models with class weighting.
6. Compare accuracy, fraud precision, fraud recall, F1-score, and confusion matrices.
7. Save the selected model, scaler, and feature-column order.

## Results
The notebook calculates the metrics when it is run on the downloaded dataset. Insert the actual results from your run into the project report before submission. Metrics can vary with data version and execution settings. Do not claim unverified values.

## GitHub repository
After creating a GitHub repository, paste its URL here: **[Add your actual GitHub repository URL]**. Do not submit this placeholder as a real repository link.

## Limitations and future scope
This is an educational prototype, not a production banking system. It does not block live transactions or guarantee fraud detection. Future improvements include threshold tuning, precision-recall curves, cross-validation, explainability, monitoring, and a secure review dashboard.
