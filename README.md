# Diabetic Readmission Prediction

This project uses real-world clinical data to predict the likelihood of hospital readmission for diabetic patients. It includes data preprocessing, exploratory analysis, feature engineering, and predictive modeling using Random Forest and XGBoost classifiers.

---

## Overview

Hospital readmissions can be costly and often preventable. Leveraging data from over 100,000 diabetic patient encounters, this project builds a predictive model to identify high-risk individuals before discharge. The objective is to assist healthcare providers in planning early interventions and improving patient outcomes.


## Objectives

- Predict whether a diabetic patient will be readmitted within 30 days.
- Identify key factors influencing readmission risk.
- Use machine learning to improve insights and support healthcare decision-making.

---

## Files

- `Diabetic_Readmission_Prediction_Polished.ipynb`: https://github.com/M-coder-cyber-02/Diabetic-Readmission-Prediction/blob/main/Diabetic_Readmission_Prediction.ipynb
- `diabetic_data.csv`: https://github.com/M-coder-cyber-02/Diabetic-Readmission-Prediction/blob/main/diabetic_data.csv
- `README.md`: https://github.com/M-coder-cyber-02/Diabetic-Readmission-Prediction/blob/main/README.md
  
---

## How to Run

```bash
git clone https://github.com/M-coder-cyber-02/Diabetic-Readmission-Prediction.git
cd Diabetic-Readmission-Prediction  
pip install -r requirements.txt 
jupyter notebook Diabetic_Readmission_Prediction_Polished.ipynb
```
---

## Methodology

- Removed multicollinear and redundant features using correlation matrix and VIF.
- Scaled numerical features using `StandardScaler`.
- Handled class imbalance using SMOTE.
- Trained an `XGBoost` classifier.
- Evaluated performance using precision, recall, F1-score, ROC-AUC, and confusion matrix.

---

## Results

- **Best Model**: XG Boost(after SMOTE and feature tuning)
- **Key Metrics**:
  - **Precision**: 1.00
  - **Recall**: 0.87
  - **F1-score**: 0.93
  - **ROC-AUC Score**: 0.958
- **Top Predictors**:
  - `total_encounters`  
  - `age`   
  - `num_procedures`    
  - `discharge_disposition_id`
  - `is_chronic`   
---

## Conclusion

This project demonstrates the potential of predictive modeling in healthcare to identify at-risk diabetic patients and reduce preventable readmissions. 


## Future Improvements

- Integrate temporal features such as time between admissions
- Apply model explainability using SHAP or LIME
- Validate using external datasets or time-split holdouts for generalizability

---

## Dataset

- **Source**: UCI Machine Learning Repository  
  [Diabetes 130-US hospitals for years 1999–2008 Data Set](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **Records**: ~100,000 hospital encounters for diabetic patients
- **Features**: Demographics, lab results, diagnoses, medications, admission/discharge details

---

## Acknowledgements

Thanks to the UCI Machine Learning Repository for providing the dataset.

---

## Contact

**Author**: Mahwish Malik  
**LinkedIn**: https://www.linkedin.com/in/dr-mahwish-m-a570892a8/
**Email**: mahwishmalik1997@gmail.com
