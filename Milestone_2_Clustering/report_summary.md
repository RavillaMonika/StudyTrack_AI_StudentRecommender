# 🎯 Milestone 2: Clustering and Pattern Detection

## 🧠 Objective
The main objective of this milestone is to identify distinct patterns among students based on their study behavior and academic performance.  
By applying clustering techniques, we can group students into meaningful clusters such as high achievers, average performers, and low-engagement learners.

---

## 📊 Dataset Information

- **Dataset Name:** `student_data.csv`
- **Source:** Derived from Milestone 1 (Student Information + Assessment Data)
- **Total Records:** Students with their study-related attributes
- **Main Features Used:**
  - `study_hours`
  - `attendance`
  - `assignments_score`
  - `exam_score`

---

## ⚙️ Steps Followed

### 1️⃣ Data Preparation
- Loaded dataset using **pandas**
- Selected key numerical columns for clustering  
- Handled missing values (if any)  
- Standardized features using **StandardScaler** from `sklearn.preprocessing`

### 2️⃣ Dimensionality Reduction
- Applied **Principal Component Analysis (PCA)** to reduce dataset to 2 components  
- Helped visualize high-dimensional data in 2D space

### 3️⃣ Clustering Technique
- Implemented **K-Means Clustering**
- Used **Elbow Method** and **Silhouette Score** to find the best number of clusters
- Fitted the model and predicted cluster labels for all students
- Added a new column `Cluster` in the DataFrame

### 4️⃣ Cluster Analysis
- Calculated average `study_hours`, `attendance`, `assignments_score`, and `exam_score` per cluster
- Compared differences between clusters using summary tables and visualizations

### 5️⃣ Visualization
- Created 3 main visualizations and saved them inside the `visualizations/` folder

---

## 🧰 Tools and Libraries Used

| Tool | Purpose |
|------|----------|
| **Python** | Main programming language |
| **Pandas** | Data loading and processing |
| **NumPy** | Numerical computation |
| **Scikit-learn** | Machine learning (scaling, PCA, K-Means) |
| **Matplotlib & Seaborn** | Visualization and graph plotting |

---

## 🖼️ Visualizations Created

| Plot Type | Description | File Name |
|------------|--------------|------------|
| **Cluster Scatter Plot (PCA)** | Shows clusters in 2D PCA space | `cluster_scatter.png` |
| **Cluster Profile Bar Chart** | Mean study, attendance, and score values per cluster | `cluster_profile_bar.png` |
| **Box Plot (Exam Score)** | Exam score variation across clusters | `boxplot_cluster_comparison.png` |
| **Cluster Size Pie Chart** | Percentage of students in each cluster | `cluster_size_pie.png` |
| **Correlation Heatmap** | Correlation among all numerical features | `correlation_heatmap.png` |

---

## 🔍 Key Insights and Interpretation

- **Cluster 0:** Students with **high study hours and scores** — consistent performers  
- **Cluster 1:** Students with **medium engagement and moderate marks** — average achievers  
- **Cluster 2:** Students with **low study time, low attendance, and low scores** — need improvement  

These clusters help in identifying different learning patterns and can guide future interventions like personalized study plans.

---

## 🧾 Summary of Findings
- K-Means clustering successfully divided students into meaningful categories.  
- PCA visualization clearly showed separation among performance groups.  
- The dataset shows a strong positive correlation between **study_hours** and **exam_score**.  
- These insights can be used to recommend study improvements or tutoring support.

