
# Chronic Kidney Disease Prediction Using Machine Learning

## Overview

This project focuses on predicting Chronic Kidney Disease (CKD) using clinical and laboratory data with machine learning techniques. The work combines manual exploratory analysis and an automated machine learning (AutoML) pipeline to build, evaluate, and compare multiple predictive models.

## Project Files

- **Untitled.ipynb**:  
  Contains manual data exploration, preprocessing, feature engineering, and initial model building.
- **Automation_Approach.ipynb**:  
  Implements an automated machine learning workflow for preprocessing, model selection, evaluation, and prediction.

## Dataset

- **Source**: Clinical and laboratory records of 400 patients.
- **Features**:  
  - Demographic: Age  
  - Clinical: Blood Pressure (`bp`), Hypertension (`htn`), Diabetes Mellitus (`dm`), Coronary Artery Disease (`cad`), Appetite (`appet`), Pedal Edema (`pe`), Anemia (`ane`)
  - Laboratory: Specific Gravity (`sg`), Albumin (`al`), Sugar (`su`), Blood Glucose Random (`bgr`), Blood Urea (`bu`), Serum Creatinine (`sc`), Sodium (`sod`), Potassium (`pot`), Hemoglobin (`hemo`), Packed Cell Volume (`pcv`), White Blood Cell Count (`wc`), Red Blood Cell Count (`rc`), etc.
  - Target: `classification` (`ckd` or `notckd`)
- **Preprocessing**:  
  - Missing value imputation (mean/mode)
  - Categorical encoding (binary/one-hot)
  - Feature scaling (MinMaxScaler)
  - Feature selection

## Approach

### Manual Workflow (`Untitled.ipynb`)

1. **Data Exploration**  
   - Inspected data types, missing values, and distributions.
   - Visualized feature relationships and target distribution.

2. **Preprocessing**  
   - Imputed missing values.
   - Encoded categorical features.
   - Scaled numerical features.

3. **Feature Engineering**  
   - Selected relevant features based on domain knowledge and correlation.

4. **Model Building**  
   - Split data into train/test sets.
   - Built and evaluated baseline models.

### Automated Workflow (`Automation_Approach.ipynb`)

1. **AutoML Setup**  
   - Automated preprocessing (imputation, encoding, scaling).
   - Stratified K-Fold cross-validation.
   - Model comparison across 10+ algorithms.

2. **Model Evaluation**  
   - Compared models using metrics: Accuracy, AUC, Recall, Precision, F1, Kappa, MCC.
   - Top models: Extra Trees, Random Forest, Gradient Boosting, XGBoost, LightGBM.

3. **Prediction**  
   - Generated predictions and probability scores for new/test data.

## Results

- **Best Model**: Extra Trees Classifier
- **Performance (10-fold CV)**:
  - **Accuracy**: ~99.6%
  - **AUC**: 1.00
  - **Recall**: ~99.3%
  - **Precision**: 100%
  - **F1 Score**: ~99.7%
- **Other Models**: Random Forest, Gradient Boosting, XGBoost, and LightGBM also performed exceptionally well.

## How to Run

1. **Clone the repository** or download both notebooks and the dataset.
2. **Install dependencies**:
   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn xgboost lightgbm
   ```
3. **Open and run the notebooks** in Jupyter Notebook or Jupyter Lab, following the cell order.
4. **Review results**:  
   - Manual analysis in `Untitled.ipynb`
   - Automated model comparison in `Automation_Approach.ipynb`

## Key Insights

- Automated machine learning can rapidly identify high-performing models for clinical prediction tasks.
- Feature scaling and proper imputation significantly improve model stability and performance.
- Ensemble models (Extra Trees, Random Forest, Gradient Boosting) are especially effective for tabular clinical data.

## Future Work

- Deploy the best model as a web API or dashboard for clinical use.
- Integrate additional patient data for improved generalization.
- Explore explainability tools (e.g., SHAP, LIME) for model transparency.

## Contact

For questions, suggestions, or collaboration, please contact:  
**[Saikat Pal]**  
**[saikatpal912@gmail.com]**  
**[@Saikat912]**

---

**Note:**  
All code and results are for educational and research purposes. For clinical deployment, further validation and regulatory compliance are required.

