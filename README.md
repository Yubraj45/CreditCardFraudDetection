# CreditCardFraudDetection
This project implements a machine learning-based fraud detection system for credit card transactions using a Random Forest classifier. The model identifies potentially fraudulent transactions with 73% recall and 93% precision, effectively catching 3 out of 4 fraud attempts while maintaining low false alarm rates.


## Model Performance (Time-Validated)

After correcting for temporal bias using chronological split validation:

| Metric | Value |
|--------|-------|
| **Fraud Detection Rate (Recall)** | 73.3% |
| **Precision** | 93.2% |
| **F1 Score** | 82.1% |
| **Optimal Threshold** | 0.35 |

**Business Impact:**
- Catches 3 out of 4 fraudulent transactions
- Only 7% of flagged transactions are false alarms
- Flags ~0.1% of all transactions for review

**Comparison with Random Split:**
Random split overestimated recall by 11 percentage points,
demonstrating the critical importance of time-based validation
for fraud detection systems.
