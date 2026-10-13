# Semiconductor Manufacturing Process — Pass/Fail Prediction

## Project Overview

This project focuses on predicting semiconductor manufacturing yield using sensor measurements. Each production example is classified as Pass or Fail based on the measured process features.

**Domain:** Semiconductor Manufacturing Process  
**Project:** Corizo Capstone Project 2

## Objective

- Explore and prepare sensor data.
- Investigate relevant features and class imbalance.
- Train and compare multiple machine-learning models.
- Evaluate the final model's ability to detect failed production examples.
- Identify limitations and opportunities for improvement.

## My Contribution

**Model Comparison, Integration and Finalization — Member 5**

My contribution includes:
- Comparing candidate machine-learning models.
- Evaluating the selected model on the test set.
- Summarizing performance metrics.
- Documenting the model recommendation and limitations.

## Model Selection

The Random Forest model was selected based on its highest cross-validation Average Precision (AP) score among the evaluated candidates.

- Cross-validation AP: 0.219
- Evaluation threshold: approximately 0.101

## Final Model Evaluation

| Metric | Result |
|---|---:|
| Test samples | 314 |
| Actual Fail cases | 21 |
| Detected Fail cases | 14 |
| Missed Fail cases | 7 |
| Accuracy | 0.720 |
| Fail precision | 0.147 |
| Fail recall | 0.667 |
| Fail F1-score | 0.241 |
| ROC-AUC | 0.764 |
| Average Precision | 0.187 |

## Interpretation and Limitations

At the selected threshold, the model detected 14 of the 21 actual Fail cases but also generated false alarms. Only 21 Fail cases were present in the test set, so the reported metrics should be interpreted cautiously.

Accuracy alone is not sufficient for this imbalanced classification problem. Further validation, feature analysis and threshold tuning may improve performance.

## Repository Structure

- `notebooks/` — model training and final evaluation notebooks.
- `results/` — model comparisons, evaluation metrics and selected hyperparameters.
- `model/` — reserved for the final trained model, if appropriate to share.

## Acknowledgment

This work was completed as part of Corizo Capstone Project 2 in the Semiconductor Manufacturing Process domain.