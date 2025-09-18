# Leukemia-Survival-Prediction
## Survival analysis of acute myeloid leukemia using statistical and machine-learning-based time-to-event models

This repository presents ongoing work for the **QRT Challenge**. The objective is to compare different survival analysis approaches applied to acute myeloid leukemia (AML). Implemented models include Cox Proportional Hazards (CoxPH) and Random Survival Forests (RSF). The project is still under development and does not represent its final version.

---

## Background
Acute myeloid leukemia (AML) is a severe hematological malignancy with highly variable patient outcomes. Accurate survival prediction is critical to guide treatment decisions and improve prognosis. Traditional approaches such as Cox proportional hazards provide a baseline reference but may not fully capture complex clinical and molecular factors. This project investigates whether modern machine-learning-based time-to-event methods can enhance survival prediction.

---

## Methods
We used a retrospective AML cohort (YYYY–YYYY) including demographic, clinical, cytogenetic, and molecular data such as FLT3, NPM1, and TP53 mutations. The outcomes studied were overall survival time and event status. Feature selection was conducted with random forests. Models were evaluated using the concordance index (C-index) and Integrated Brier Score (IBS), and Kaplan–Meier curves were produced for different risk groups.

---

## Preliminary Results
Preliminary analyses identified age, FLT3 mutation status, and cytogenetic classification as the most influential predictors. Random Survival Forests slightly outperformed CoxPH in terms of predictive accuracy (C-index around 0.75). The models reproduced known clinical trends: favorable cytogenetics corresponded to the best survival outcomes, while adverse-risk cytogenetics and TP53 mutations were associated with the poorest. These results remain preliminary and will be refined in subsequent iterations.

---

## Conclusion
Classical statistical models and machine-learning survival methods show promising performance for AML prognosis. Further work will focus on hyperparameter optimization, external validation, and improved risk stratification. This repository reflects a **work in progress** for the QRT Challenge.

---

## Installation

```bash
pip install -r requirements.txt
