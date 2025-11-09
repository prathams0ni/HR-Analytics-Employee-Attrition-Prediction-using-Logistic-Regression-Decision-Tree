# HR Analytics Employee Attrition Prediction using Logistic Regression & Decision Tree

A comprehensive machine learning project to predict employee attrition. This project leverages Logistic Regression and Decision Tree algorithms to analyze HR data, achieving up to 99% validation accuracy. It covers the full data science pipeline from EDA and preprocessing to model deployment on unseen data.

## 📊 Project Overview
This project tackles the critical business problem of employee attrition by building predictive machine learning models. Using an HR dataset, we analyze various factors that contribute to an employee's decision to leave the company. The goal is to create a model that can accurately identify employees at risk of attrition, allowing for proactive retention strategies.

The project follows a complete data science lifecycle:
1.  **📥 Data Loading & Exploration**
2.  **🧹 Data Preprocessing & Cleaning**
3.  **🔍 Exploratory Data Analysis (EDA)**
4.  **⚙️ Feature Engineering & Selection**
5.  **🤖 Model Building & Evaluation** (Logistic Regression & Decision Tree)
6.  **🧪 Validation on Unseen Test Data**

## 📁 Dataset
The dataset (`HR_file.csv`) contains 14,999 entries with 11 attributes related to employee information and their work experience.

**📋 Features Include:**
- `Satisfaction Level` 😊
- `Last Evaluation` 📝
- `Number of Projects` 📂
- `Monthly Hours` ⏰
- `Total Time at the Company` 📅
- `Work Accidents` 🚧
- `Quit the Company` 🚪 (Target Variable)
- `Promoted in Last 5 yrs` 📈
- `Departments` 🏢
- `salary` 💰 (Categorical: low, medium, high)
- `Management` 👨‍💼

## 🚀 Project Steps & Methodology

### 1. 🧹 Data Preprocessing
- **🔍 Handling Duplicates:** Identified and removed 1,463 duplicate entries to ensure data integrity, resulting in a clean dataset of 13,536 records.
- **❓ Missing Values:** The dataset contained no null values, so no imputation was necessary.
- **✅ Data Integrity:** Checked for anomalies or inconsistent values in all columns; none were found.

### 2. 🔍 Exploratory Data Analysis (EDA)
- **📊 Department-wise Salary Distribution:** Visualized the distribution of salary tiers across different departments. **Key insight:** The Management department has the highest number of low-salary employees.

### 3. ⚙️ Feature Engineering & Selection
- **🔤 Encoding Categorical Variables:** Applied Label Encoding to transform categorical features (`Departments`, `salary`) into a numerical format suitable for machine learning algorithms.
- **🎯 Feature Selection:** Utilized a correlation matrix to identify and select the most relevant features for predicting attrition, helping to reduce noise and improve model performance.
- **📈 Multicollinearity Check:** Analyzed the correlation between independent variables to ensure the model's stability and interpretability.

### 4. 🎯 Data Splitting & Scaling
- The data was split into **training** and **testing** sets to evaluate model performance fairly.
- **⚖️ Feature Scaling:** Applied `StandardScaler` to normalize the feature space, which is crucial for models like Logistic Regression that are sensitive to the scale of data.

### 5. 🤖 Model Building & Evaluation

#### **📉 Model 1: Logistic Regression**
- A fundamental classification algorithm was implemented as a baseline model.
- **📊 Results:**
  - **Training/Validation Accuracy:** An impressive **98%** accuracy was achieved on the validation set, indicating an excellent fit to the training data.

#### **🌳 Model 2: Decision Tree Classifier**
- Implemented to capture non-linear relationships and compare performance against Logistic Regression.
- **📊 Results:**
  - **Training/Validation Accuracy:** Achieved a near-perfect **99%** accuracy on the validation set, demonstrating the model's high capability to learn from the data.

### 6. 🧪 Testing on Unseen Data
To ensure the models' generalizability and avoid overfitting, a separate, unseen test dataset was created and used for final evaluation.

- **📉 Logistic Regression on Unseen Data:** Accuracy of **84%** ✅
- **🌳 Decision Tree on Unseen Data:** Accuracy of **84%** ✅

**💡 Key Insight:** While the Decision Tree performed slightly better on the validation set, both models generalized to the unseen data with the same **84% accuracy**. This indicates that the models are robust and effective at predicting employee attrition on new, real-world data, with the Decision Tree showing a marginal edge in learning complexity.

## 🎯 Key Findings & Business Implications
- 🎯 The models successfully identified key factors leading to employee attrition.
- ✅ The high accuracy on unseen data (**84%**) confirms the model's reliability for practical deployment.
- ⚠️ The Management department's high count of low-salary employees is a critical area for HR to investigate for improving retention.

## 🛠️ Technologies Used
- **🐍 Python**
- **📚 Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## 📈 Model Performance Summary

| Model                | Validation Accuracy | Unseen Test Accuracy |
|----------------------|--------------------|----------------------|
| Logistic Regression  | 98%                | 84%                  |
| Decision Tree        | 99%                | 84%                  |

Both models performed impressively, indicating a robust preprocessing pipeline and feature selection process.

## 🏃‍♂️ How to Run
1.  📥 Clone the repository.
2.  🔧 Ensure the required libraries are installed (`pip install -r requirements.txt`).
3.  ▶️ Run the `HR Project Solution.ipynb` Jupyter notebook to execute the entire analysis.

## 🎓 Conclusion
This project demonstrates a robust end-to-end pipeline for predicting employee attrition. By comparing multiple algorithms, we developed a highly accurate model that can serve as a powerful tool for HR departments to reduce turnover and retain valuable talent. The **84% accuracy on unseen data** proves the model's practical utility in real-world scenarios.

---

**⭐ If you find this project useful, don't forget to give it a star.
