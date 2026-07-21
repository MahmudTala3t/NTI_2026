# Employee Attrition Analysis

## Project Overview

This project focuses on exploring, cleaning, and preprocessing an Employee Attrition dataset to prepare it for machine learning. The objective is to understand the dataset, identify the factors that may influence employee attrition, and transform the raw data into a clean and structured format suitable for predictive modeling.

---

## Project Workflow

### 1. Data Exploration
- Loaded the dataset and inspected its structure.
- Examined the number of rows and columns.
- Identified numerical and categorical features.
- Checked data types using `info()`.
- Generated descriptive statistics using `describe()`.
- Explored unique values for categorical variables.

---

### 2. Data Cleaning
- Identified missing values in each column.
- Removed or handled missing values where appropriate.
- Removed duplicate records to improve data quality.
- Verified the dataset after cleaning.

---

### 3. Outlier Detection
- Analyzed numerical features for extreme values.
- Applied the Interquartile Range (IQR) method to detect outliers.
- Removed observations outside the acceptable range while preserving meaningful employee records.

---

### 4. Feature Encoding
Since machine learning models require numerical input, categorical variables were converted into numerical representations.

Encoding techniques included:
- Binary encoding for columns such as:
  - Attrition
  - OverTime
- Numerical encoding for categorical features including:
  - Gender
  - Department
  - BusinessTravel

---

### 5. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand the characteristics of employees and identify patterns related to attrition.

#### Numerical Analysis
- Examined distributions of numerical features.
- Calculated summary statistics.
- Visualized data using:
  - Histograms
  - Box plots
  - Correlation heatmaps

#### Categorical Analysis
- Analyzed the frequency distribution of categorical variables.
- Compared employee attrition across different categories.
- Used count plots and pie charts to visualize categorical distributions.

---

### 6. Correlation Analysis
- Computed the correlation matrix for numerical variables.
- Visualized correlations using a heatmap.
- Identified features strongly associated with employee attrition.
- Examined correlations between independent variables to detect potential multicollinearity.

---

### 7. Relationship Analysis
Investigated the relationship between important employee characteristics and attrition, including:

- Age
- Monthly Income
- Job Level
- Total Working Years
- Years at Company
- OverTime
- Training Times Last Year

Visualization techniques such as box plots and distribution plots were used to compare employees who stayed with those who left.

---

## Key Insights

During the analysis, several important observations were identified:

- Employees working overtime showed a higher likelihood of leaving the company.
- Higher monthly income was generally associated with lower attrition.
- Older and more experienced employees tended to remain with the company.
- Job level was strongly related to monthly income and total working years.
- Training frequency showed only a weak linear relationship with employee attrition.
- Some features exhibited strong correlations, indicating possible redundancy for certain machine learning models.

---

## Outcome

After completing the preprocessing pipeline, the dataset became:

- Clean and free from duplicate records.
- Processed for missing values.
- Reduced in the presence of extreme outliers.
- Fully encoded into numerical features.
- Ready for feature selection, model training, and machine learning classification tasks.

This processed dataset can be used to build predictive models such as Logistic Regression, Decision Trees, Random Forest, XGBoost, and other classification algorithms.