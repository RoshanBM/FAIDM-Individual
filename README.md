# Diabetes Risk Analysis - FAIDM Individual Project

## Roshan Balaji Mahashabde (u5735905)
---
## Project Overview

This project conducts a comprehensive analysis of diabetes risk factors using the CDC Diabetes Health Indicators Dataset. The analysis employs multiple data mining techniques including exploratory data analysis, clustering, classification, and association rule mining to identify risk patterns and predict diabetes outcomes.

## Dataset

**Source:** CDC Diabetes Health Indicators Dataset  
**Size:** ~253,680 records with 22 features  
**Target Variable:** `Diabetes_012` (0=No Diabetes, 1=Prediabetes, 2=Diabetes)

## Project Structure

```
diabetes-risk-analysis/
├── data/
│   ├── raw/                    # Original CDC dataset
│   └── processed/              # Cleaned and transformed datasets
├── notebooks/
│   ├── 01_eda_and_prep.ipynb          # Data exploration and preparation
│   ├── 02_clustering_analysis.ipynb   # K-Means and K-Prototypes clustering
│   ├── 03_classification_model.ipynb  # Binary classification models
│   └── 04_classification_multi.ipynb  # Multi-class classification
├── models/                     # Saved model artifacts
├── outputs/
│   └── figures/               # Visualization outputs
└── requirements.txt           # Python dependencies
```

## Notebooks

### 1. Data Preparation & EDA (`01_eda_and_prep.ipynb`)
- Statistical profiling and correlation analysis
- Feature engineering (Metabolic Syndrome Index, Physical Distress Ratio, etc.)
- Data preprocessing and scaling
- PCA transformation for dimensionality reduction
- Creation of datasets for clustering, classification, and association rule mining

### 2. Clustering Analysis (`02_clustering_analysis.ipynb`)
- K-Means clustering with PCA visualization
- K-Prototypes clustering for mixed data types
- Silhouette analysis and cluster profiling
- Patient persona identification

### 3. Binary Classification (`03_classification_model.ipynb`)
- Binary diabetes prediction (Diabetic vs Non-Diabetic)
- Multiple algorithms: Logistic Regression, Random Forest, XGBoost, SVM
- Handling class imbalance with SMOTE
- Model evaluation with ROC-AUC, precision-recall metrics

### 4. Multi-class Classification (`04_classification_multi.ipynb`)
- Three-class prediction (Healthy, Prediabetes, Diabetes)
- Advanced ensemble methods
- Feature importance analysis
- Comprehensive performance evaluation

## Key Features

- **Composite Health Indicators:** Metabolic Syndrome Index, Physical Distress Ratio, Healthy Habit Score
- **Dimensionality Reduction:** PCA for efficient clustering
- **Class Imbalance Handling:** SMOTE resampling for minority classes
- **Multiple Modeling Approaches:** Supervised and unsupervised learning techniques

## Requirements

```
pandas
numpy
scikit-learn
imbalanced-learn
matplotlib
seaborn
xgboost
```

Install dependencies:
```bash
pip install -r diabetes-risk-analysis/requirements.txt
```

## Usage

1. **Data Preparation:**
   Run `01_eda_and_prep.ipynb` to load, explore, and prepare the data

2. **Clustering Analysis:**
   Execute `02_clustering_analysis.ipynb` for patient segmentation

3. **Classification:**
   - Run `03_classification_model.ipynb` for binary classification
   - Run `04_classification_multi.ipynb` for multi-class prediction

## Key Findings

- Strong correlation between General Health, BMI, High Blood Pressure, and diabetes risk
- Significant class imbalance requiring specialized resampling techniques
- Identification of distinct patient segments for targeted interventions
- Non-linear relationships justify ensemble methods over simple linear models

## Author

FAIDM Individual Project - University of Warwick

## License

Academic project for educational purposes.