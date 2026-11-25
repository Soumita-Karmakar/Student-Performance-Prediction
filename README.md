# Student Performance Prediction and Academic Risk Analysis

## 📌 Project Overview

The **Student Performance Prediction and Academic Risk Analysis** project uses Machine Learning techniques to analyze student academic data, predict final examination marks, identify academic risk levels, and understand the factors influencing student performance.

The project aims to support the identification of students who may need additional academic attention through data analysis and predictive modelling.

## 🎯 Project Objectives

- Predict students' final academic examination marks.
- Classify student performance into different academic categories.
- Identify students' academic risk levels.
- Segment students into performance groups using clustering.
- Identify the major factors influencing student performance.
- Allow users to enter student details and obtain predictions.

## 📂 Project Structure

```text
Student-Performance-Prediction/
│
├── dataset/
│   ├── student_performance_challenge33.csv.xlsx
│   └── README.md
│
├── student_performance_analysis.ipynb
│
└── README.md
```

## 📊 Dataset Description

The project uses a student performance dataset containing approximately 5,003 records and 10 columns.

### Dataset Features

| Feature | Description |
|---|---|
| Student_ID | Unique student identifier |
| Attendance_Percentage | Student attendance |
| Internal_Marks | Internal examination marks |
| Assignment_Score | Assignment performance |
| Previous_Semester_Score | Previous semester marks |
| Study_Hours_Per_Day | Daily study hours |
| Engagement_Level | Student engagement level |
| Final_Academic_Score | Final academic marks |
| Performance_Band | Academic performance category |
| Performance_Change | Change in academic performance |

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

- Checked and removed duplicate records.
- Handled missing values.
- Encoded categorical engagement levels.
- Detected and capped outliers in numerical features.
- Prepared input features and target variables for Machine Learning.

## 🤖 Machine Learning Algorithms

Four Machine Learning techniques were implemented.

### 1. Linear Regression
Used to predict students' final academic examination marks based on academic and engagement-related features.

### 2. Logistic Regression
Used to classify students into four performance categories:
- At Risk
- Average
- Good
- Excellent

### 3. K-Nearest Neighbors (KNN)
Used to classify student performance based on similarities in academic characteristics.

### 4. K-Means Clustering
Used to group students into three clusters based on academic features and identify lower, medium, and higher-performing groups.

## 📈 Model Evaluation Results

| Model | Evaluation Metric | Result |
|---|---|---:|
| Linear Regression | R² Score | 0.672 |
| Linear Regression | MAE | 4.07 |
| Linear Regression | RMSE | 5.12 |
| Logistic Regression | Accuracy | 58.14% |
| KNN | Accuracy | 53.55% |
| K-Means | Silhouette Score | 0.114 |

**Note:** The classification models have limited performance, particularly for minority performance categories. K-Means also shows weak cluster separation. These limitations are considered when interpreting the results.

## 📉 Data Visualization and Analysis

The project includes visualizations for:

- Distribution of student performance.
- Actual vs. predicted examination marks.
- Classification model accuracy comparison.
- Academic risk distribution.
- Student performance clusters.
- Permutation feature importance.

## 🎓 Academic Risk Analysis

Academic risk is identified using predicted final examination marks.

| Predicted Marks | Academic Risk |
|---|---|
| Below 40 | High Risk |
| 40 to below 60 | Medium Risk |
| 60 and above | Low Risk |

These thresholds are illustrative and can be adjusted according to institutional grading criteria.

## 🔍 Feature Importance

Permutation Feature Importance is used to identify the most influential input features.

The observed feature importance ranking is:

1. Internal Marks
2. Study Hours Per Day
3. Previous Semester Score
4. Attendance Percentage
5. Engagement Level
6. Assignment Score

These values indicate the influence of each feature on the trained Linear Regression model's predictive performance.

## 💻 User Input Prediction

The project includes an interactive user-input section where users can enter:

- Attendance Percentage
- Internal Marks
- Assignment Score
- Previous Semester Score
- Study Hours Per Day
- Engagement Level

### Final Prediction Output

The system provides:

1. Predicted final examination marks.
2. Pass/Fail indication derived from predicted marks using a passing threshold of 40.
3. Academic risk level (Low, Medium, High).
4. Student performance segmentation using K-Means.
5. Identification of major factors affecting student performance.

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Machine Learning

## ▶️ How to Run the Project

1. Clone or download this repository.
2. Open `student_performance_analysis.ipynb` using Google Colab or Jupyter Notebook.
3. Upload or access the dataset.
4. Update the dataset file path in the notebook if necessary.
5. Run the notebook cells sequentially.
6. Enter student academic details in the user-input section to obtain predictions.

## 🚀 Future Improvements

- Improve classification performance for minority student categories.
- Explore additional feature engineering techniques.
- Improve cluster separation and interpretation.
- Validate academic risk thresholds using institutional grading standards.
- Develop a web-based interface for student performance prediction.

## 👩‍💻 Author

**Soumita Karmakar**

MCA Student | Brainware University

GitHub: [Soumita-Karmakar](https://github.com/Soumita-Karmakar)

---

*This project was developed as part of academic work on Machine Learning and Student Performance Analysis.*
