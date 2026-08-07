# Telco Customer Churn Prediction Pipeline (Final Project)

**Author:** Dana Bolden  
**Course:** ITAI 1371 – 12321  
**Problem Type:** Binary Classification  

## Overview
This repository contains a complete, production-grade machine learning pipeline designed to predict customer churn. The project emphasizes rigorous data hygiene, advanced multi-column feature engineering, absolute data leakage prevention, and multi-model ensemble comparisons.

## Repository File Structure
```text
├── README.md                          # Project documentation
├── Final_Exam.ipynb                   # Main reproducible Google Colab notebook
├── master_comparison_table.csv        # Raw model metrics export
├── master_comparison_table.pdf        # Styled comparison table deliverable
├── ensemble_test_results.csv          # Final ensemble test metrics
├── Reflection_Journal_Timothy.pdf     # Personal project reflection journal
├── Final_Project_Report.pdf           # Comprehensive written project report
└── Telco Churn dataset.xlsx           # Raw dataset (or download link)

```

## Key Technical Achievements

1. **Data Audit & Repair:** Identified and corrected hidden string space corruptions in the `TotalRevenue` financial records, followed by median imputation to maintain structural matrix integrity.
2. **Feature Engineering:** Built high-level compound behavioral attributes (`Total_AddOn_Services`, `Total_Calls_All_Types`) avoiding weak unit conversions and adhering to strict rubric standards.
3. **Leakage-Free Resampling:** Implemented a strict 70/15/15 stratified partition paired with isolated training-set SMOTE balancing and scaling.
4. **Ensemble Superiority:** Trained and validated 6 base classifiers, combining the top three (Gradient Boosting, Tuned Random Forest, SVC) into a Soft Voting Ensemble, achieving a robust **0.945 Test ROC-AUC**.

## How to Run

1. Open `Final_Exam.ipynb` in Google Colab or your local Jupyter environment.
2. Ensure the raw dataset `Telco Churn dataset.xlsx` is uploaded to the root working directory.
3. Select **Runtime > Restart and run all** to execute the pipeline from ingestion to final ensemble evaluation.

```

```
