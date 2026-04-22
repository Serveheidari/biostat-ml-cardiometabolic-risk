# biostat-ml-cardiometabolic-risk
End-to-end biostatistical and machine learning project analyzing cardiometabolic risk in NHANES using regression, classification, PCA, clustering, and hypothesis testing.

# Biostatistical and Machine Learning Approaches to Cardiometabolic Risk Prediction in NHANES

##  Overview
This project integrates **biostatistical modelling** and **machine learning** techniques to analyze cardiometabolic risk factors using NHANES data.

The goal is to:
- Identify key predictors of cardiometabolic risk
- Compare statistical and machine learning approaches
- Explore population heterogeneity using unsupervised learning

---

## Methods Used

### Statistical Methods
- Multiple Linear Regression
- Poisson Regression
- Hypothesis Testing (t-test)

### Machine Learning
- Logistic Regression (with coefficient interpretation)
- K-Nearest Neighbors (KNN)
- Random Forest (feature importance)

### Unsupervised Learning
- Principal Component Analysis (PCA)
- KMeans Clustering (with cluster profiling)

---

## Dataset

Data was obtained from NHANES:

- Demographics (DEMO):  
  https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/DEMO_J.XPT

- Body Measures (BMI):  
  https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/BMX_J.XPT

- Blood Pressure:  
  https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/BPX_J.XPT

- Laboratory (Glucose & Cholesterol):  
  https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/GLU_J.XPT  
  https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/TCHOL_J.XPT

---

## Key Findings

- **BMI, age, and glucose** are consistently associated with cardiometabolic risk
- Poisson regression shows **BMI as the strongest contributor** to cumulative risk
- Logistic Regression achieved **AUC ≈ 0.80**, indicating good discrimination
- Non-linear models (**KNN, Random Forest**) outperform linear models
- Clustering reveals **distinct cardiometabolic subgroups**
- Hypothesis testing confirms **significantly higher BMI in diabetic individuals**

---

## Visualizations

The project includes:
- Distribution plots
- Correlation heatmaps
- PCA projections
- ROC curves
- Feature importance plots
- Cluster visualizations

---

## Limitations

- Risk score is a constructed variable (not clinical outcome)
- Limited predictors (no lifestyle variables)
- Feature importance is predictive, not causal
- Moderate model performance reflects complexity of health data

---

## Future Work

- Incorporate behavioral and socioeconomic variables
- Use clinically validated outcomes (e.g., HbA1c)
- Apply advanced interpretability methods (SHAP)
- Validate models on external datasets

---

## How to Run

```bash
git clone https://github.com/YOUR_USERNAME/biostat-ml-cardiometabolic-risk.git
cd biostat-ml-cardiometabolic-risk
pip install -r requirements.txt
jupyter notebook
