# 📊 Customer Churn Prediction using Machine Learning

Predicting customer churn is vital for businesses to improve retention and lifetime value. This project analyzes customer service patterns and builds supervised Machine Learning models to accurately predict whether a customer is likely to discontinue their subscription/service.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.x
* **Environment:** Google Colab / Jupyter Notebook
* **Data Handling:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, XGBoost

---

## 📁 Project Structure & Workflow

1. **Data Ingestion & Cleaning:**
   * Handled missing values in `TotalCharges`.
   * Converted target column `Churn` into binary values (1 = Churned, 0 = Retained).
   * Applied One-Hot Encoding on categorical features.

2. **Exploratory Data Analysis (EDA):**
   * Visualized target class distribution.
   * Computed and plotted top correlation factors influencing churn.

3. **Model Development:**
   * **Logistic Regression** (Standardized using `StandardScaler`)
   * **Random Forest Classifier**
   * **XGBoost Classifier**

4. **Model Evaluation:**
   * Models evaluated on **Accuracy**, **Recall**, and **ROC-AUC Score**.
   * Evaluated false negatives via **Confusion Matrix** and **ROC Curves**.

---

## 📈 Key Results & Metrics

| Model Name | Accuracy | Recall | ROC-AUC Score |
| :--- | :--- | :--- | :--- |
| **Logistic Regression** | ~80.1% | ~54.2% | ~0.84 |
| **Random Forest** | ~79.5% | ~51.8% | ~0.83 |
| **XGBoost** | ~78.8% | ~52.5% | ~0.82 |

*(Note: Exact metrics may slightly vary depending on data splits.)*

---

## 💡 Key Business Insights
* **Contract Type:** Customers on Month-to-Month contracts have a significantly higher churn rate compared to One-Year or Two-Year contracts.
* **Tenure:** Newer customers (low tenure) are most vulnerable to churning.
* **Services:** Fiber Optic users and non-tech support subscribers show higher churn risk.

---

## 🚀 How to Run the Project

1. Clone this repository or download the `.ipynb` file.
2. Open **Google Colab** or Jupyter Notebook.
3. Upload `Customer_Churn_Prediction_Project.ipynb`.
4. Upload the dataset (`telco_churn_dataset.csv`) when prompted.
5. Run all cells sequentially to reproduce the analysis, graphs, and predictions.
6. 
