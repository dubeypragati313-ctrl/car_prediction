# 🚗 Car Price Prediction App

An interactive Machine Learning web application built with **Streamlit** that predicts the estimated selling price of used cars based on technical specifications (such as mileage, engine capacity, power, fuel type, etc.).

---

## ✨ Key Features

- **Dynamic UI Generation:** Input controls (number inputs and dropdowns) are dynamically generated based on the dataset's numerical and categorical features.
- **Automated Data Cleaning & Parsing:** 
  - Extracts numeric values from unit strings (e.g., extracting `20.5` from `"20.5 kmpl"` or `1197` from `"1197 CC"`) using regular expressions (`re`).
  - Automatically handles missing values using median imputation for numerical data and mode imputation for categorical data.
- **Robust ML Pipeline:** Uses `Scikit-Learn`'s `Pipeline` and `ColumnTransformer` to seamlessly combine preprocessing (`StandardScaler`, `OneHotEncoder`) with a `Linear Regression` model.
- **Cached Operations:** Utilizes `@st.cache_data` and `@st.cache_resource` for fast performance, avoiding re-loading data or re-training the model on every user interaction.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Web Framework:** Streamlit
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-Learn (`LinearRegression`, `Pipeline`, `ColumnTransformer`, `SimpleImputer`, `OneHotEncoder`, `StandardScaler`)

---

## 📂 Installation & Setup

Follow these steps to run the application locally on your machine:

### 1. Install Requirements
Make sure you have Python installed, then install the necessary dependencies:

```bash
pip install -r requirements.txt
