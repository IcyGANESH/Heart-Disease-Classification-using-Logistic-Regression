# 🫀 Heart Disease Classification using Logistic Regression

This project aims to build a classification model to detect the presence of heart disease based on various medical parameters. The project includes data preprocessing, visualization, model training, evaluation, and performance analysis.

---

## 📁 Dataset

The dataset used is [`heart_disease_uci.csv`](./heart_disease_uci.csv), which includes several clinical features such as:

- Age
- Sex
- Chest pain type (cp)
- Resting blood pressure (trestbps)
- Serum cholesterol (chol)
- Fasting blood sugar (fbs)
- Resting ECG results (restecg)
- Maximum heart rate achieved (thalach)
- Exercise-induced angina (exang)
- ST depression induced by exercise (oldpeak)
- Slope of the peak exercise ST segment (slope)
- Number of major vessels (ca)
- Thalassemia (thal)
- Target (presence of heart disease)

---

## 🧪 Technologies Used

- **Python**
- **Pandas, NumPy** for data manipulation
- **Matplotlib, Seaborn** for visualization
- **Scikit-learn** for machine learning modeling

---

## 🧼 Data Preprocessing

- Removed whitespace in column names
- Converted categorical columns using Label Encoding
- Replaced `?` with NaN and filled using median values
- Converted target to binary:  
  `0 = No Heart Disease`, `1 = Heart Disease`

---

## 📊 Exploratory Data Analysis (EDA)

- **Correlation Heatmap**: Shows feature correlations  
- **Target Countplot**: Class balance check  
- **Histograms**: Distribution of numerical features

---

## 🧠 Model

### Logistic Regression

- Features standardized using `StandardScaler`
- Dataset split into train/test (80/20)
- Model trained using `LogisticRegression` from scikit-learn

---

## 📈 Model Evaluation

- **Accuracy Score**
- **Classification Report**: Precision, Recall, F1-Score
- **Confusion Matrix**: TP, TN, FP, FN
- **ROC Curve and AUC Score** for binary classification

---

## 📌 Results Summary

- **Model**: Logistic Regression  
- **Accuracy**: _Insert Accuracy_  
- **AUC Score**: _Insert AUC_  

Model shows promising performance for heart disease detection using clinical data.

---

## 📍 Future Work

- Try advanced models like Random Forest, XGBoost
- Perform feature selection and dimensionality reduction
- Use cross-validation and hyperparameter tuning
- Deploy using Flask/Streamlit for interactive use

---

## 📂 Run Locally

```bash
git clone https://github.com/your-username/heart-disease-classification.git
cd heart-disease-classification
pip install -r requirements.txt
python heart_disease_model.py
