# Leukemia-Survival-Prediction
## Survival analysis of acute myeloid leukemia using machine learning and deep-learning-based time-to-event models

This repository presents ongoing work conducted as part of the **QRT Challenge**. The objective is to compare classical and modern approaches to survival analysis applied to acute myeloid leukemia (AML). Several time-to-event survival prediction models are implemented, including Cox Proportional Hazards (CoxPH), Random Survival Forests (RSF), DeepSurv, and DeepHit. The project remains under development, and this repository does not represent its final version.

---

## Background
Acute myeloid leukemia (AML) is an aggressive hematological malignancy characterized by the uncontrolled clonal proliferation of myeloid precursors. Accurate survival prediction for AML patients is essential to guide treatment decisions and improve clinical outcomes. Conventional statistical approaches such as Cox proportional hazards often fail to capture complex non-linear interactions between molecular and clinical features. This project investigates whether machine learning and deep-learning-based time-to-event models can provide more accurate and robust predictions of survival outcomes in AML.

---

## Materials and Methods
The study relies on a retrospective cohort of patients diagnosed with AML between YYYY and YYYY. The dataset includes demographic variables such as age and sex, clinical variables including white blood cell count, blast percentage, and treatment types, as well as cytogenetic abnormalities and recurrent gene mutations such as FLT3, NPM1, and TP53. The outcome variables are overall survival time, measured in months, and the event indicator (death or censored).

Feature importance was first assessed using a random forest approach. The models developed include Cox Proportional Hazards, Random Survival Forests, DeepSurv, and DeepHit. Model performance was evaluated using the concordance index (C-index) and the Integrated Brier Score (IBS). Kaplan–Meier survival curves were produced for clinically relevant subgroups defined by cytogenetic and molecular risk classifications.

---

## Preliminary Results
Random forest feature selection identified age, FLT3 mutation status, and cytogenetic risk group as the most influential predictors of survival. Early experiments suggest that DeepSurv and DeepHit achieve better predictive performance than CoxPH and RSF, with C-index values ranging between 0.76 and 0.78. Predicted survival outcomes were consistent with clinical expectations: patients with favorable cytogenetic profiles had the highest survival probabilities, while those with adverse-risk cytogenetics or TP53 mutations experienced the lowest. FLT3-ITD positive patients showed poor prognosis unless targeted therapies were administered. These findings remain preliminary and will be refined as the project progresses.

---

## Conclusion and Next Steps
The first results indicate that deep-learning-based survival models, in particular DeepSurv and DeepHit, may provide an advantage over traditional methods in AML prognosis. The project is still ongoing and future steps will include further hyperparameter optimization, external validation using independent datasets, and the integration of treatment response prediction. This repository therefore reflects a work-in-progress version developed for the QRT Challenge.

---

## Installing Requirements

```bash
pip install -r requirements.txt
