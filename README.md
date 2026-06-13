# CodeAlpha_Credit-Scoring-Model

## Files

| File | Task | Dataset | Models |
|---|---|---|---|
| `task1_credit_scoring.py` | Credit Scoring Model | Synthetic financial dataset (generated in-script, saved to CSV) | Logistic Regression, Decision Tree, Random Forest |

## How to run

```bash
python3 task1_credit_scoring.py

All required libraries (`numpy`, `pandas`, `scikit-learn`, `matplotlib`)
are standard and install with:

```bash
pip install numpy pandas scikit-learn matplotlib
```
## Important honesty notes (please read before submitting)

1. **Task 1 (Credit Scoring):** No real credit dataset was provided in the
   brief, so a synthetic-but-realistic dataset (income, debts, loan
   amounts, payment history, etc.) is generated programmatically. If your
   mentor expects a specific real dataset (e.g., the German Credit dataset
   or a Kaggle credit-scoring dataset), swap the data-generation block for
   `pd.read_csv("your_dataset.csv")` — the rest of the pipeline (scaling,
   train/test split, model training, metrics) will work unchanged.

## Results summary (from the runs in this environment)

 **Task 1 — Credit Scoring:** Logistic Regression performed best
  (Accuracy 0.88, ROC-AUC 0.96). `debt_to_income` and
  `late_payments_last_year` were the strongest predictors — consistent
  with real-world credit risk models.

## Risks / limitations to be aware of

- All accuracy numbers will vary slightly between runs unless random
  seeds are fixed (they are, here, via `random_state=42`).  
