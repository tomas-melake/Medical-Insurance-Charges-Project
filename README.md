# Medical-Insurance-Charges-Project

Predicting medical insurance charges using Linear Regression. Full end‑to‑end machine learning workflow including data extraction, preparation, modeling, evaluation, visualization, and interpretation. Data Science Capstone Project.

---

##  Overview  
This project builds a complete machine learning pipeline to predict **medical insurance charges** using demographic and lifestyle features. The workflow includes:

- Data extraction  
- Data cleaning & preparation  
- Feature engineering  
- Train/test splitting  
- Feature scaling  
- Linear Regression modeling  
- Model evaluation  
- Coefficient interpretation  
- Visualization  
- Summary & implications  

The project demonstrates a transparent, interpretable, and industry‑aligned approach to predictive modeling.

---

##  Research Question  
**How accurately can a linear regression model predict medical insurance charges using patient characteristics such as age, BMI, smoking status, sex, number of children, and region?**

---

##  Hypothesis  
- **Null Hypothesis (H₀):** No statistically significant relationship exists between patient characteristics and medical insurance charges.  
- **Alternative Hypothesis (H₁):** Patient characteristics significantly influence medical insurance charges.

---

##  Dataset  
The dataset used is the WGU‑provided **Insurance and Medical Costs Data.xlsx**, containing:

- Age  
- Sex  
- BMI  
- Number of children  
- Smoking status  
- Region  
- Medical charges  

Raw data is **not uploaded** to GitHub to maintain professional and ethical standards.

---

##  Data Extraction  
Data was loaded from Excel using `pandas.read_excel()` with proper header handling.  
Initial inspection included:

- `.info()`  
- `.describe()`  
- Missing value checks  

---

##  Data Preparation  
Key steps:

- Standardizing categorical text  
- One‑hot encoding (`OneHotEncoder`)  
- Train/test split (80/20)  
- Feature scaling (`StandardScaler`)  
- Saving prepared datasets for reproducibility  

Prepared outputs include:

- `prepared_dataset.csv`  
- `X_train.csv`, `X_test.csv`  
- `y_train.csv`, `y_test.csv`  
- `X_train_scaled.csv`, `X_test_scaled.csv`

---

##  Model Training  
A **Linear Regression** model was trained using scaled features.

Model file saved as:

- `linear_regression_model.pkl`

---

##  Model Evaluation  
Metrics used:

- **R² Score:** ~0.784  
- **RMSE:** ~5796  
- **MAE:** ~4181  

These results indicate strong predictive performance for a real‑world healthcare cost dataset.

---

##  Visualization  
A scatter plot compares **actual vs predicted** charges, with a red dashed perfect‑prediction line.

This helps visually assess model accuracy and identify outliers.

---

##  Coefficient Analysis  
Model coefficients reveal how each feature influences medical charges.  
This supports interpretability and aligns with industry expectations for transparent models.

---

##  Summary & Implications  
- Linear Regression performs well for this dataset.  
- Smoking status, BMI, and age show strong influence on charges.  
- The model explains ~78% of cost variation.  
- Results support the use of regression for insurance pricing strategies.

---

##  Limitations  
- Dataset cannot be expanded (WGU‑provided).  
- No additional real‑world variables (e.g., chronic conditions, income).  
- Linear Regression may not capture nonlinear relationships.

---

##  Recommendations  
- Explore advanced models (Random Forest, Gradient Boosting).  
- Add more predictors if available.  
- Perform hyperparameter tuning.  
- Conduct cross‑validation for robustness.

---

##  Future Work  
- Deploy model using Flask or FastAPI  
- Build interactive dashboards (Streamlit)  
- Add SHAP value analysis for deeper interpretability  

---

##  Project Structure  
Medical-Insurance-Charges-Project/
│
├── notebooks/
│   └── Medical Insurance Charges Project.ipynb
│
├── scripts/
│   ├── C.1_Data_Extraction.py
│   ├── C.2_Data_Preparation.py
│   ├── C.3_Model_Training.py
│   └── C.4_Model_Coefficients.py
│
├── results/
│   ├── prepared_dataset.csv
│   ├── X_train.csv
│   ├── X_test.csv
│   ├── y_train.csv
│   ├── y_test.csv
│   ├── X_train_scaled.csv
│   └── X_test_scaled.csv
│
├── models/
│   └── linear_regression_model.pkl
│
└── README.md

---

##  Tools & Technologies  
- Python  
- Pandas  
- NumPy  
- Scikit‑Learn  
- Matplotlib  
- Jupyter Notebook  

---

##  References  
Western Governors University — Data Science Capstone Dataset & Guidelines.


