# SummerOfCode_Batch2_Day3
# Bank Marketing Campaign Analysis

## Overview

This project analyzes a bank marketing dataset to predict whether clients will subscribe to a term deposit (binary classification task). The dataset contains information about bank clients and their responses to marketing campaigns.

## Dataset

The dataset (`bank-full.csv`) contains 45,211 entries with 17 features including:
- Client demographics (age, job, marital status, education)
- Financial information (default history, balance, housing loan, personal loan)
- Campaign details (contact type, day, month, duration, campaign contacts)
- Previous campaign outcomes (pdays, previous, poutcome)
- Target variable (`y` - whether the client subscribed to a term deposit)

## Project Structure

1. **Data Exploration**: Initial inspection and analysis of the dataset structure and contents
2. **Data Preprocessing**:
   - Handling missing values
   - Encoding categorical variables (Label Encoding and One-Hot Encoding)
   - Feature scaling (StandardScaler)
   - Train-test split (80-20 ratio)

3. **Model Building**:
   - Logistic Regression (baseline model)
   - Decision Tree
   - Random Forest
   - Gradient Boosting
   - Ensemble methods

4. **Evaluation**:
   - Accuracy scores
   - Classification reports
   - Confusion matrices

## Key Findings

- The dataset is imbalanced (39,922 "no" vs 5,289 "yes" responses)
- Logistic Regression achieved 89.87% accuracy with good precision for class "no" (92%) but lower precision for class "yes" (65%)
- Decision Tree showed slightly lower overall accuracy (87.08%) but more balanced performance between classes

## How to Use

1. Clone the repository
2. Install required packages: `pandas`, `scikit-learn`, `seaborn`, `matplotlib`
3. Run the Jupyter notebook (`summerofcode__B2__D3.ipynb`)

## Future Work

- Address class imbalance with techniques like SMOTE or class weighting
- Feature engineering to improve model performance
- Hyperparameter tuning for better results
- Experiment with neural networks
- Deploy the best model as a predictive service

## Dependencies

- Python 3.x
- Jupyter Notebook
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## License

This project is open source and available under the MIT License.

## Acknowledgments

Data source: [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) from UCI Machine Learning Repository
