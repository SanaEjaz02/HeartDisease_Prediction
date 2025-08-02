Heart Disease Prediction using Logistic Regression

📊 Objective
This project aims to predict whether a person is at risk of heart disease based on their medical attributes using a Logistic Regression model. The dataset used is the UCI Cleveland Heart Disease Dataset.

📁 Dataset
- Source: [UCI Heart Disease Dataset (Kaggle)]
- Records: 297 patients
- Target: `condition` (0 = No Heart Disease, 1 = Heart Disease Present)

🧠 Features Used
| Feature        | Description |
|----------------|-------------|
| age            | Age of the patient |
| gender         | 0 = Female, 1 = Male |
| cp             | Chest Pain Type (0-3) |
| trestbps       | Resting Blood Pressure (mm Hg) |
| chol           | Serum Cholesterol (mg/dl) |
| fbs            | Fasting Blood Sugar > 120 mg/dl (1 = True) |
| restecg        | Resting Electrocardiographic Results |
| thalach        | Maximum Heart Rate Achieved |
| exang          | Exercise-induced Angina (1 = Yes) |
| oldpeak        | ST depression induced by exercise |
| slope          | Slope of the peak exercise ST segment |
| ca             | Number of major vessels (0-3) colored by fluoroscopy |
| thal           | 0 = Normal, 1 = Fixed Defect, 2 = Reversible Defect |
| condition      | Target Variable (0 = No Disease, 1 = Disease Present) |

📝 Steps Performed
1. Data Loading & Cleaning
    - Loaded CSV dataset.
    - Checked for null/missing values.
2. Exploratory Data Analysis (EDA)
    - Visualized feature distributions.
    - Created correlation heatmap.
3. Data Preprocessing
    - Split data into Train & Test sets (80/20 split).
    - Applied StandardScaler for feature scaling.
4. Model Training
    - Trained a Logistic Regression model.
5. Model Evaluation
    - Evaluated using:
        - Accuracy Score
        - Confusion Matrix
        - Classification Report (Precision, Recall, F1-Score)
        - ROC-AUC Curve
6. Feature Importance Analysis
    - Analyzed feature coefficients to see their influence on predictions.

---

📈 Results
- Accuracy Score:  0.73
- ROC AUC Score: 0.84
- Most impactful features:
  Feature  Coefficient
11        ca     1.178408
1     gender     0.874545
12      thal     0.744396

🛠 Libraries Used
- Python 3.x
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

📂 Files Included
- `Heart_Disease_Prediction.ipynb` — Colab Notebook with code & visualizations.
- `README.md` — This documentation.


📣 Conclusion
A simple Logistic Regression model can effectively predict heart disease presence based on a patient's health attributes. Future improvements could include trying advanced models like Random Forest, XGBoost, and hyperparameter tuning.


