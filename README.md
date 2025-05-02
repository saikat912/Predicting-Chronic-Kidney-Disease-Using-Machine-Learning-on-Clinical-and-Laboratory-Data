# Chronic Kidney Disease Prediction Using Machine Learning

## Project Overview

This project aims to predict the presence of Chronic Kidney Disease (CKD) in patients based on various clinical and laboratory features using machine learning techniques. Early detection of CKD can significantly improve patient outcomes by enabling timely treatment and management.

The dataset contains multiple features such as age, blood pressure, specific gravity, albumin levels, sugar levels, red blood cell count, and many others collected from patients. The goal is to build a robust predictive model to classify whether a patient has CKD or not.

## Dataset

- The dataset consists of 400 records with 26 columns representing patient attributes and the target classification.
- Features include both numerical and categorical variables such as:
  - Age, Blood Pressure (bp), Specific Gravity (sg), Albumin (al), Sugar (su)
  - Red Blood Cell count (rbc), Pus Cell (pc), Pus Cell Clumps (pcc), Bacteria (ba)
  - Blood Glucose Random (bgr), Blood Urea (bu), Serum Creatinine (sc), Sodium (sod), Potassium (pot)
  - Hemoglobin (hemo), Packed Cell Volume (pcv), White Blood Cell count (wc), Red Blood Cell count (rc)
  - Hypertension (htn), Diabetes Mellitus (dm), Coronary Artery Disease (cad), Appetite (appet), Pedal Edema (pe), Anemia (ane)
- The target variable is `classification` with two classes: `ckd` and `notckd`.

## Technologies Used

- Python 3.x
- Libraries:
  - pandas, numpy for data manipulation
  - seaborn, matplotlib for data visualization
  - scikit-learn for machine learning model building and evaluation
  - warnings to handle warnings during execution

## Project Structure

- `16th_Feb_25_HealthCare-Domain-Project.ipynb` - Jupyter notebook containing the complete exploratory data analysis, preprocessing, model training, and evaluation.
- Dataset (embedded or external CSV file as applicable)

## Key Steps in the Project

1. **Data Loading and Exploration**  
   Understanding the dataset, checking for missing values, data types, and initial statistics.

2. **Data Cleaning and Preprocessing**  
   Handling missing values, encoding categorical variables, and scaling numerical features using MinMaxScaler.

3. **Exploratory Data Analysis (EDA)**  
   Visualizing feature distributions and relationships using seaborn and matplotlib.

4. **Feature Selection**  
   Identifying the most relevant features for predicting CKD.

5. **Model Training and Evaluation**  
   Splitting data into training and testing sets, training machine learning models (e.g., Logistic Regression, Random Forest, etc.), and evaluating performance metrics such as accuracy, precision, recall, and F1-score.

6. **Conclusion and Insights**  
   Summarizing findings and model effectiveness.

## How to Run

1. Clone the repository or download the notebook file.
2. Ensure you have Python 3.x installed.
3. Install required libraries (if not already installed):
   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn
   ```
4. Open the Jupyter notebook `16th_Feb_25_HealthCare-Domain-Project.ipynb` in Jupyter Lab or Jupyter Notebook.
5. Run the notebook cells sequentially to reproduce the analysis and results.

## Future Work

- Improve model accuracy by trying advanced algorithms like XGBoost or deep learning.
- Deploy the model as a web application for real-time CKD prediction.
- Incorporate more patient data for better generalization.

## Contact

For questions or suggestions, please contact:  
[Saikat Pal]  
[saikatpal912@gmail.com]  
[https://www.linkedin.com/me?trk=p_mwlite_feed-secondary_nav]

---

If you want, I can also help you generate a shorter or more technical README version. Just let me know!

