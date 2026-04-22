# Diabetes Classification using Decision Trees

## Project Overview
Decision tree classifier to predict diabetes diagnosis based on clinical measurements from the Pima Indians Diabetes Database.

## Dataset
- 768 observations of women aged 21+
- 9 variables (8 predictors + 1 target)
- Class distribution: 268 diabetic (34.9%), 500 non-diabetic (65.1%)

## Analysis Highlights

### Preprocessing Strategies Tested
8 different approaches compared:
- Base 1: Original data (baseline)
- Base 2: Remove zero values
- Base 3: Global mean imputation
- Base 4: Global median imputation
- Base 5: MICE imputation
- Base 6: Conditional median imputation ⭐ (Selected)
- Base 7: MICE + SMOTE
- Base 8: Conditional median + SMOTE

### Results (Best Model - Base 6)
- **F1-Score: 0.591** (primary metric for imbalanced data)
- Accuracy: 77.9%
- Precision: 63.8%
- Recall: 55.6%
- AUC-ROC: 0.753
- Cross-validation (5-fold): 0.591 ± 0.053

### Top Features
1. Glucose (38.4%)
2. Insulin (21.6%)
3. Age (18.3%)

## Key Findings
- Glucose concentration and insulin levels are primary diabetes indicators
- Outcome-conditional median imputation preserves data while handling missing values effectively
- Decision tree provides interpretable, clinically actionable rules
- Model shows stable performance across cross-validation folds

## Recommendations
- Use as screening tool, not replacement for clinical diagnosis
- Adjust classification threshold based on clinical requirements
- Validate on external datasets before deployment
- Monitor performance periodically for data drift

## Files
- `decision_tree_diabetes.ipynb`: Complete analysis notebook
- `diabetes.csv`: Dataset
- `requirements.txt`: Python dependencies
- `README.md`: This file

## How to Run

```bash
# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook decision_tree_diabetes.ipynb
```

## Technologies
- Python 3.x
- scikit-learn
- pandas, numpy
- matplotlib, seaborn
- imbalanced-learn (SMOTE)

## Author
Cleane Santos | Data Science & Statistician

---
*This project demonstrates practical machine learning workflow: EDA → preprocessing → model comparison → evaluation → interpretation.*
