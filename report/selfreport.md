Smart Life Decision System (Study + Health + Finance + Food)

 A single platform (website/app)
 Multiple independent modules(4 modules)
 Each solves a real-life problem
 All presented in one unified interface


---------------------------------------------------------------------------------------------------------------------------

🌐 Website (Streamlit App)
            |
      📊 Master Dataset
            |
 -------------------------------------------------
 |              |              |                 |
📚 Study      🏥 Health     💰 Spending      🍽️ Food
 |              |              |                 |
EDA           EDA            EDA               EDA
 |              |              |                 |
Outlier       Outlier        Outlier           (Optional)
Detection     Detection      Detection
 |              |              |                 |
SDA           SDA            SDA               Rule-Based
 |              |              |                 |
ML Model     Health Score   Spending Pattern   Diet Quality
(Regression)  (Derived)      (Derived)          (Category)
 |              |              |                 |
Prediction    Insight        Insight           Insight
 -------------------------------------------------
            |
     🧠 Combined Decision Engine
            |
   🎯 Final Recommendations to User

---------------------------------------------------------------------------------------------------------------------------

This system integrates multiple aspects of daily life into a single decision-support platform, providing data-driven insights and actionable recommendations to improve overall lifestyle.

---------------------------------------------------------------------------------------------------------------------------

🌐 One Website → Multiple Life Modules
🏠 Homepage

“Choose your need”

A unified platform where users analyze different aspects of student life:

Study 📚
Health 🏥
Spending 💰
Food 🍽️

📚 Module 1: Study & Productivity Analyzer
🎯 Purpose:
To analyze academic behavior and predict student performance

🔍 What it does:
Analyzes study hours, screen time, stress, and past performance
Identifies patterns affecting academic results
📈 Features:
Predicts exam score using Linear Regression
Detects low productivity trends
💡 Suggestions:
“Increase study hours for better performance”
“Reduce screen time and distractions”


🏥 Module 2: Health & Lifestyle Analyzer
🎯 Purpose:
To evaluate lifestyle-based health and its impact on academic performance

🔍 What it does:
Analyzes sleep, stress, mental health, and activity levels
Computes a composite health score
📈 Features:
Categorizes students into Low / Medium / High health
Identifies relationship between health and academic performance
💡 Suggestions:
“Improve sleep schedule for better performance”
“Reduce stress and maintain balanced lifestyle”


💰 Module 3: Spending & Saving Analyzer
🎯 Purpose:
To understand financial behavior and its effect on student lifestyle

🔍 What it does:
Analyzes spending patterns based on income and part-time work
Detects high or unnecessary spending
📈 Features:
Categorizes spending into Low / Medium / High
Identifies spending patterns affecting productivity
💡 Suggestions:
“Control unnecessary expenses”
“Maintain a balanced spending habit”


🍽️ Module 4: Food & Nutrition Analyzer
🎯 Purpose:
To assess diet quality and its role in student well-being

🔍 What it does:
Uses diet quality data to evaluate eating habits
Identifies unhealthy dietary patterns
📈 Features:
Classifies diet as Healthy / Average / Unhealthy
Links food habits with overall lifestyle
💡 Suggestions:
“Improve diet quality for better health”
“Maintain a balanced nutritional intake”


🧠 Final Output of System

👉 Each module provides:
📊 Insights (EDA + SDA)
📈 Predictions (only in Study Module)
💡 Actionable Suggestions
🔥 Combined Decision Engine

All modules are integrated to generate:
👉 Final personalized recommendations

🎯 Final Impact

The system helps users:
Improve academic performance 📚
Maintain better health 🏥
Manage finances effectively 💰
Develop healthier eating habits 🍽️

---------------------------------------------------------------------------------------------------------------------------

DATASET:

Google Dataset Search:
👉 https://datasetsearch.research.google.com

📚 Module 1: Study & Productivity Analyzer

https://datasetsearch.research.google.com/search?src=0&query=student%20habits%20dataset&docid=L2cvMTF5d3N0N2J3cg%3D%3D
https://www.kaggle.com/datasets/aryan208/student-habits-and-academic-performance-dataset

🏥 Module 2: Health & Lifestyle Analyzer

https://datasetsearch.research.google.com/search?src=0&query=lifestyle%20dataset&docid=L2cvMTFsXzRqMHE0bg%3D%3D
https://www.kaggle.com/datasets/adilshamim8/sleep-cycle-and-productivity

student
https://datasetsearch.research.google.com/search?src=0&query=lifestyle%20dataset%20of%20student&docid=L2cvMTF6MTc1dmNndw%3D%3D
https://www.kaggle.com/datasets/jay7080dev/student-lifestyle-data

💰 Module 3: Spending & Saving Analyzer

https://datasetsearch.research.google.com/search?src=0&query=student%20personal%20expense%20dataset&docid=L2cvMTF5M2xfenc1dg%3D%3D
https://www.kaggle.com/datasets/sumanthnimmagadda/student-spending-dataset

🍽️ Module 4: Food & Nutrition Analyzer
https://www.kaggle.com/datasets/trolukovich/nutritional-values-for-common-foods-and-products

---------------------------------------------------------------------------------------------------------------------------
WORKING:

learned how to use jupiter notebook as well during this project.


📚 MODULE 1: STUDY & ACADEMIC PERFORMANCE ANALYSIS
worked on the module 1 dataset and created a report sugggession for each student based on their sleep, study how, result and many other colums.
-EDA
-Linear Regression
-Recommendation System


The Study Module focuses on analyzing student academic behavior and predicting exam performance using machine learning techniques. This module forms the core of the system, as it directly models the relationship between study habits and academic outcomes.

📊 Data Used

The following features were selected from the dataset:

Study Hours per Day
Previous GPA
Screen Time
Stress Level
Mental Health Rating
Exam Score (Target Variable)
⚙️ Data Preprocessing
Removed unnecessary columns to reduce noise
Handled missing values (if any)
Standardized column names
Created derived feature:
Screen Time = Social Media Hours + Netflix Hours
📈 Exploratory Data Analysis (EDA)

EDA was performed to understand patterns in student behavior:

Study hours showed a near-normal distribution
Higher study hours correlated with higher exam scores
Increased screen time negatively impacted performance
📉 Outlier Detection & Handling
Outliers were identified using boxplots
IQR (Interquartile Range) method was applied
Extreme values were handled using capping
🤖 Model Implementation
Linear Regression model was implemented
Dataset was split into training and testing sets
Model was trained to predict exam scores
📊 Model Performance
R² Score ≈ 0.87
Mean Absolute Error ≈ 3.19

This indicates strong predictive capability and high accuracy.

🧠 Insights
Study hours and previous GPA are strong predictors of performance
Screen time and stress negatively influence exam scores
Academic performance is influenced by multiple lifestyle factors


🏥 MODULE 2: HEALTH & LIFESTYLE ANALYSIS (UPDATED)

The Health Module evaluates the impact of lifestyle factors on student academic performance. Instead of using a separate dataset, a composite health index was derived from available features in the primary dataset to maintain data consistency.

📊 Data Used
The following health-related features were used:
Sleep Hours
Stress Level
Mental Health Rating
Exercise Frequency
Social Activity

⚙️ Health Score Construction
A composite Health Score was created using a weighted formula based on domain knowledge.

📊 Health Score Calculation Weights
Factor	Weight	Impact Type
Sleep Hours	+8	Positive
Mental Health Rating	+10	Positive
Exercise Frequency	+6	Positive
Social Activity	+2	Positive
Stress Level	-7	Negative

🧮 Formula
The health score is calculated as:
Health Score = 
(8 × Sleep Hours) +
(10 × Mental Health Rating) +
(6 × Exercise Frequency) +
(2 × Social Activity) -
(7 × Stress Level)

🧠 Explanation
Higher sleep and mental well-being improve the score
Regular exercise contributes positively to physical health
Social interaction has a moderate positive effect
Stress negatively impacts overall health

👉 This creates a balanced lifestyle-based health index

🔄 Normalization
The health score was normalized to a range of 0 to 1 to ensure consistency and comparability across students.
🏷️ Categorization
Students were grouped into:
Low Health
Medium Health
High Health

📊 Analysis
The relationship between health and academic performance was analyzed:
Students with higher health scores achieved higher exam scores
A clear upward trend was observed across health categories
📈 Key Results
Health Category	Average Exam Score
Low	86.01
Medium	89.03
High	91.63

🧠 Insights
Health has a direct positive influence on academic performance
Balanced lifestyle leads to improved outcomes
High stress significantly reduces performance


