# EdTech Student Learning & Performance Analytics

---

## 📘 Overview

This project analyzes a dataset of 14,000+ student records to understand **learning behaviors, engagement patterns, and academic performance**. The focus is on identifying factors that influence student success, segmenting learners into profiles, and providing insights for improving retention and adaptive learning strategies.

- **Project Repo:** [GitHub Link](https://github.com/Chitranshi-18/Student-Learning-Performance-Analytics)

---

## 🛠️ Tools & Technologies

- **Python**: Pandas, NumPy, Matplotlib, Seaborn, SciPy, StatsModels, scikit-learn, imbalanced-learn  
  - Data cleaning, EDA, clustering, statistical analysis
- **Power BI**: Interactive dashboards for performance distribution, retention trends, and cluster visualization
- **Statistics**: ANOVA, OLS regression, correlation analysis
- **Machine Learning**: K-Means clustering, PCA for dimensionality reduction

---

## 🗂️ Dataset Structure

- **Source:** Merged from two publicly available Kaggle datasets  
- **Records:** 14,003 anonymized student records  
- **Features (16 attributes):**
  - **Study behaviors & engagement:** StudyHours, Attendance, Extracurricular, AssignmentCompletion, OnlineCourses, Discussions
  - **Resource access & environment:** Resources, Internet, EduTech
  - **Motivation & psychological factors:** Motivation, StressLevel
  - **Demographics:** Gender, Age (18–30)
  - **Learning preference:** LearningStyle
  - **Academic performance:** ExamScore, FinalGrade

---

## 🚀 Project Workflow

### **1. Data Loading & Inspection**
- Imported datasets and merged into a unified CSV (`merged_dataset.csv`)  
- Checked data types, missing values, and duplicates  
- Saved cleaned dataset (`merged_dataset_cleaned.csv`) for analysis

### **2. Data Cleaning & Preprocessing**
- Removed duplicates and handled missing values  
- Encoded categorical variables using LabelEncoder  
- Scaled features using:
  - **Z-score standardization** for statistical tests and PCA  
  - **Min-Max normalization** for clustering

### **3. Exploratory Data Analysis (EDA)**
- Visualized distributions of engagement, motivation, and performance metrics  
- Identified patterns and correlations between engagement and exam/final grades  

### **4. Clustering Analysis**
- Applied **K-Means clustering** to segment learners into profiles  
- Determined optimal cluster number using **Elbow Method** and **Silhouette Score**  
- Evaluated cluster quality with **Silhouette Score** and **Davies–Bouldin Index**  

### **5. Dimensionality Reduction & Visualization**
- Used **PCA** to reduce feature dimensions for 2D/3D visualization  
- Explored feature importance in distinguishing clusters  

### **6. Mapping Clusters to Learning Styles**
- Associated each cluster with dominant learning style based on feature patterns  

### **7. Statistical Analysis**
- Conducted **ANOVA** to test significant differences in FinalGrade and ExamScore across clusters  
- Built **OLS regression models** to evaluate impact of engagement factors on performance  

### **8. Final Dataset**
- Saved fully processed dataset with clusters and scaled features: `merged_dataset_final.csv`  
- Ready for **Power BI dashboards** and further analysis

---

## 📊 Key Metrics & Findings

**Clusters reveal distinct learner profiles:**
- **Cluster 0:** Moderate engagement, balanced performance  
- **Cluster 1:** High extracurricular involvement, slightly lower grades  
- **Cluster 2:** Low engagement in discussions but good assignment completion  
- **Cluster 3:** Mixed engagement, slightly lower online course participation  

**Statistical Insights:**
- ANOVA confirmed significant differences in **FinalGrade** (F = 5.07, p < 0.01) and **ExamScore** (F = 3.21, p < 0.05) across clusters  
- Regression identified **Discussions** and **AssignmentCompletion** as significant predictors of FinalGrade

---

## 📝 Future Improvements

- Build **interactive Power BI dashboards** to visualize:
  - Cluster-specific engagement and performance  
  - Age/gender distribution across learning profiles  
  - Trends in ExamScore and FinalGrade  
- Implement **predictive models** for student dropout risk and performance forecasting  
- Incorporate **cohort or temporal analysis** for longitudinal insights

---
