# Anomaly-Detection-for-Financial-Transactions
This project builds an unsupervised anomaly detection system to identify fraudulent transactions in a highly imbalanced financial dataset. The Credit Card Fraud Detection dataset contains 284,807 transactions of which only 492 are fraudulent, roughly 0.17% of the data. Standard classification fails here because predicting everything as normal already gives 99.8% accuracy. The goal instead is to learn what normal looks like and flag deviations.

Two approaches are compared: Isolation Forest, which detects anomalies by randomly partitioning the feature space and flagging points that isolate quickly, and Local Outlier Factor, which flags points that are significantly less dense than their neighbours. Both are evaluated using precision, recall, and F1-score, with confusion matrices and anomaly score distribution plots to interpret behaviour. In fraud detection recall matters more than precision, missing a fraud is more costly than a false alarm.


Built with Python, Scikit-learn, NumPy, Pandas, Matplotlib, and Seaborn.
