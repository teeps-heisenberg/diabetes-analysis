# 🩺 Diabetes Prediction with Logistic Regression

This project aims to predict the likelihood of diabetes in patients using logistic regression based on medical and lifestyle features.

## 📁 Dataset Overview

The dataset contains **100,000 samples** and the following features:

- `gender`: Male/Female  
- `age`: Patient's age  
- `hypertension`: 0 (No) / 1 (Yes)  
- `heart_disease`: 0 (No) / 1 (Yes)  
- `smoking_history`: Smoking status (e.g., never, current, former)  
- `bmi`: Body Mass Index  
- `HbA1c_level`: Glycated hemoglobin level  
- `blood_glucose_level`: Measured glucose level  
- `diabetes`: Target variable (0 = No, 1 = Yes)  

## 🔍 Project Pipeline

### 1. 📥 Data Loading
- The dataset is loaded from a CSV file using `pandas`.
- Memory usage and shape are reported.

### 2. 📊 Exploratory Data Analysis
- Visualizations with `matplotlib` and `seaborn` to understand feature distributions and relationships.
- Summary statistics and correlations are explored.

### 3. 🧹 Data Preprocessing
- Categorical features are encoded using `LabelEncoder`.
- Features are standardized using `StandardScaler`.

### 4. 🤖 Model Training
- A `LogisticRegression` model is trained to classify diabetes presence.
- `train_test_split` is used to create training and testing datasets.

### 5. ✅ Evaluation
- Model performance is assessed using:
  - Accuracy Score  
  - Classification Report  
  - Confusion Matrix  
  - ROC-AUC Score  

### 6. 📈 ROC Curve
- A Receiver Operating Characteristic (ROC) curve is plotted to visualize the tradeoff between sensitivity and specificity.

## 📦 Installation & Setup

Install all required Python packages:

```bash
pip install pandas numpy scikit-learn nltk spacy matplotlib seaborn
Download required NLTK resources:
import nltk
nltk.download('stopwords')
nltk.download('punkt')
nltk.download('punkt_tab')

## 💡 Business Value

This model provides a foundation for automated diabetes screening tools. By identifying high-risk individuals early, healthcare providers can implement lifestyle interventions and targeted care to reduce the long-term burden of the disease.

## 👤 Author

Developed by the project author as a Jupyter-based machine learning analysis for health-focused prediction.
