# 📊 Student Lifestyle & Academic Performance Analysis (Python)

## 🚀 Project Overview
This project explores how various student lifestyle factors influence academic performance using statistical analysis and machine learning techniques in Python.

The analysis is based on a real-world dataset sourced from **Kaggle**, focusing on identifying significant and non-significant factors affecting exam scores.

---

## 🎯 Objectives
- Analyze the relationship between lifestyle factors and academic performance  
- Apply statistical techniques to validate hypotheses  
- Build a regression model to predict exam scores  
- Derive meaningful, data-driven insights  

---

## 📂 Dataset
- Source: **Kaggle – Student Habits and Academic Performance Dataset**  
- The dataset includes:
  - study_hours_per_day  
  - exam_score  
  - stress_level  
  - sleep_hours  
  - diet_quality  
  - financial_status  
  - health_score  
  - monthly_spending  

- Multiple datasets were merged into a final dataset using `student_id`.

---

## 🛠️ Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- SciPy  

---

## 🔄 Data Preprocessing
- Handling missing values (median & mode imputation)  
- Data type correction and encoding  
- Feature engineering (performance levels, group categorization)  
- Outlier detection using IQR and boxplots  
- Outliers retained to preserve real-world variability  

---

## 📊 Exploratory Data Analysis (EDA)
- Summary statistics  
- Distribution analysis  
- Correlation analysis  
- Scatter plots for relationship visualization  
- Outlier detection and interpretation  

---

## 📈 Statistical Analysis

### 1. Linear Regression
- Predicted exam scores using:
  - study hours  
  - stress level  
  - sleep hours  

### 2. T-Test (Study Hours)
- Compared above-average vs below-average study groups  

### 3. T-Test (Stress Level)
- Compared low-stress vs high-stress groups  

### 4. Chi-Square Test (Diet vs Performance)
- Tested association between diet quality and performance category  

### 5. T-Test (Financial Status)
- Compared saving vs overspending students  

---

## 🔍 Key Insights
- 📈 Study hours have a strong positive impact on exam performance  
- 📉 Stress level significantly reduces academic performance  
- 😴 Sleep shows a moderate positive effect  
- 🍽️ Diet quality shows limited association  
- 💰 Financial status has no strong direct impact  

---

## 📌 Conclusion
The analysis highlights that **study habits and stress levels** are the most influential factors affecting academic performance. Other lifestyle factors play a secondary or indirect role.

---

## 📎 Project Structure
project/
│
├── data/
│ ├── raw/
│ └── processed/
│
├── notebooks/
│
├── reports/
│
└── README.md

---

## 📚 References
- Kaggle Dataset  
- Python Documentation  
- Scikit-learn Documentation  

---

## 💡 Future Scope
- Apply advanced machine learning models  
- Use larger and more diverse datasets  
- Build real-time prediction systems  
- Explore deeper causal relationships  

---

## 📊 Dashboard Overview

To complement the statistical analysis, an interactive dashboard was designed to visually represent key insights from the dataset. The dashboard provides an intuitive way to explore relationships between lifestyle factors and academic performance.

---

## 🎯 Dashboard Objectives
- Visualize key relationships such as study hours vs exam score  
- Identify patterns and trends in student behavior  
- Provide an interactive way to explore data insights  
- Support findings from statistical analysis with visual evidence  

---

## 📈 Key Visualizations

- **Scatter Plot:** Study Hours vs Exam Score (with trend line)  
- **Scatter Plot:** Stress Level vs Exam Score  
- **Bar Chart:** Average Exam Score by Study Groups  
- **Box Plot:** Exam Score distribution across Stress Levels  
- **Bar Chart:** Performance comparison by Financial Status  

---

## 🔍 Key Insights from Dashboard
- Students who study more tend to score higher  
- Higher stress levels are associated with lower performance  
- Performance differences between financial groups are minimal  
- Data distribution shows variability across different lifestyle factors  

---

## 🧠 Purpose of Dashboard
The dashboard enhances the analytical findings by providing a visual and interactive representation of the data. It helps in better understanding patterns that may not be immediately obvious through statistical outputs alone.

---

## 📌 Note
The dashboard is based on the same processed dataset used for statistical analysis, ensuring consistency between visual insights and analytical results.
---

## 🙏 Acknowledgement
Special thanks to **Dr. Karandeep Kaur** and **Dr. Mrinalini Rana** for their guidance and support throughout this project.

## ⭐ If you found this useful, consider giving it a star!
