Divorce Prediction Analysis
Project Overview

This project analyzes the key factors that predict divorce using a dataset of 5,000 couples containing demographic, psychological, relational, and behavioral variables. The study applies Exploratory Data Analysis (EDA), Principal Component Analysis (PCA), and Logistic Regression to identify the most influential predictors of divorce and to test statistically meaningful hypotheses.

The primary research question is:
Which factors—such as communication, financial stress, trust, and infidelity—most strongly predict the likelihood of divorce?

Dataset

Size: 5,000 couples

Target Variable: divorced (0 = not divorced, 1 = divorced)

Features include:

Demographic: age at marriage, number of children, income, education, employment

Relational: communication, trust, conflict frequency, conflict resolution style

Psychological: mental health issues, financial stress, social support

Behavioral: infidelity, domestic violence history, counseling attendance

Marital background: marriage type, religious compatibility, pre-marital cohabitation

Methodology

Data Preprocessing

One-hot encoding of categorical variables

Feature scaling using StandardScaler

Separation of predictors and target variable

Exploratory Data Analysis (EDA)

Distribution analysis of numerical and categorical variables

Correlation heatmaps

Boxplots comparing predictors by divorce status

Principal Component Analysis (PCA)

Dimensionality reduction to address multicollinearity

Retained 23 components explaining ~86% of total variance

Identification of dominant latent factors

Logistic Regression

Applied to PCA-transformed data

Evaluation using accuracy, precision, recall, and confusion matrix

Hypothesis testing using coefficients, p-values, and odds ratios

Key Findings

Strongest predictors of divorce:

Financial stress

Infidelity

Trust

Communication quality

Social support

Financial stress was statistically significant (p < 0.001) and increased the odds of divorce by approximately 6.4% per unit increase.

PCA revealed latent dimensions related to relationship instability, psychosocial compatibility, and marital background.

The logistic regression model achieved ~60% accuracy but showed limited recall for divorced cases due to class imbalance.

Limitations

Imbalanced dataset (more non-divorced than divorced couples)

Simplified psychological measures

Cross-sectional data (no temporal dynamics)

Potential cultural and societal bias

Repository Structure
├── data/
│   └── divorce_df.csv
├── notebooks/
│   └── DivorcePredictionModel.ipynb
├── figures/
│   ├── correlation_heatmap.png
│   ├── boxplots.png
│   ├── pca_heatmap.png
│   ├── confusion_matrix.png
├── report/
│   ├── Divorce_Prediction_Analysis_Report.pdf
├── README.md

Technologies Used

Python

pandas

NumPy

scikit-learn

matplotlib

seaborn

LaTeX (for report formatting)


Author

Haidar Saleh
