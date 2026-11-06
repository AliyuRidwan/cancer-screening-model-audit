# Cancer Screening Model Audit

Can you trust a 97.7% accurate cancer-screening model? This project audits one on a public dataset and shows why a single accuracy number isn't enough.

## Key findings
- At the default 0.5 threshold, the model scores 97.7% accuracy but misses 8 of 212 cancers.
- At 0.2 it misses 4 cancers and raises 21 false alarms. At 0.1 it misses 3 and raises 37.
- The strongest signals are concave points, perimeter and radius.
- The dataset has no demographic fields, so it can't show whether it represents patients in Lagos, Abuja or Atlanta.

## Data
UCI Breast Cancer Wisconsin (Diagnostic), a public dataset: 569 patients, 30 measurements each, 212 malignant.

## Method
Standardized logistic regression with 5-fold cross-validated predictions, a confusion matrix rebuilt at 19 thresholds, and standardized effect sizes (Cohen's d).

## Files
- `cancer-screening-model-audit.ipynb`: the full analysis
- `breast_cancer_wisconsin_public.csv`: the dataset

## Run it
Open the notebook in Google Colab and choose Runtime > Run all.

## Links
- Interactive dashboard: [add your link]
- Write-up: [add your link]

Author: Ridwan Aliyu | BI & Data Analytics | linkedin.com/in/ridwan-aliyu

*Educational analysis on public data. Not medical advice.*
