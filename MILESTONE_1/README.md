# Milestone 1: Data Preprocessing and Exploratory Data Analysis

## Objective
Analyze student performance data by joining student demographics with assessment scores to identify patterns, relationships, and insights that can inform educational strategies.

## Dataset Source
**Open University Learning Analytics Dataset (OULAD)**
- URL: https://analyse.kmi.open.ac.uk/open_dataset
- Tables Used:
  - `studentInfo.csv`: Student demographics and final results (32,593 records)
  - `studentAssessment.csv`: Assessment submissions and scores (173,912 records)
- Join Key: `id_student`

## Steps Followed

### 1. Data Loading and Exploration
- Loaded two CSV files using pandas
- Explored data structure, types, and quality
- Identified common join key (`id_student`)

### 2. Data Joining
- Used `pd.merge()` with inner join on `id_student`
- Combined demographic and performance data
- Reduced dataset to matched records only

### 3. Data Preprocessing
- **Missing Values**: Removed rows with missing scores, filled other gaps
- **Duplicates**: Identified and removed duplicate records
- **Data Types**: Converted scores to numeric, standardized categorical data
- **Encoding**: Applied Label Encoding for binary variables, One-Hot Encoding for nominal categories

### 4. Descriptive Analysis
- Generated summary statistics (mean, median, std deviation)
- Calculated correlation matrix for numeric features
- Identified outliers using IQR method
- Analyzed categorical variable distributions

### 5. Exploratory Data Analysis (EDA)
Created comprehensive visualizations:
- **Distribution Plots**: Score histogram, gender distribution, age patterns
- **Relationship Analysis**: Score vs previous attempts, performance by demographics
- **Correlation Heatmap**: Feature relationships and dependencies
- **Advanced Visualizations**: Violin plots and count plots for deeper insights

## Tools Used
- **Python 3.x** with Jupyter Notebook
- **Libraries**: 
  - pandas (data manipulation)
  - numpy (numerical operations)
  - matplotlib (plotting)
  - seaborn (statistical visualization)
  - scikit-learn (preprocessing)

## Key Insights

### Student Performance Patterns
- Average assessment score: [X.X] (fill in your actual result)
- Score distribution shows [describe pattern - normal, skewed, etc.]
- [X]% of students achieve passing grades

### Demographic Relationships
- Gender distribution: [X]% female, [X]% male students
- Age range: [X-X] years with average [X.X] years
- Strong/weak correlation between age and performance: [describe]

### Assessment Patterns
- Number of previous attempts correlates [positively/negatively/not significantly] with current scores
- Students with [characteristic] tend to perform better/worse
- Outliers represent [X]% of the dataset, indicating [interpretation]

## Visualizations Summary
1. **Distribution Analysis**: 4 charts showing score, gender, age, and box plot distributions
2. **Relationship Plots**: Scatter and bar charts revealing performance correlations
3. **Correlation Matrix**: Heatmap identifying feature interdependencies
4. **Advanced Analysis**: Violin and count plots for categorical insights
