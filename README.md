# Titanic_datset_Cleaning

# Cleaned Titanic Dataset for Predictive Modeling

This project involves cleaning and preprocessing the Titanic dataset to prepare it for machine learning models. The cleaned dataset is provided as a CSV file and includes key feature engineering steps for predictive analysis.

---

## Project Overview

The Titanic dataset is one of the most popular datasets in the data science community. This project focuses on:
- Handling missing values.
- Encoding categorical variables.
- Scaling numerical data.
- Feature engineering to enhance predictive power.

The final output is a cleaned dataset saved as `cleaned_titanic.csv`.

---

## Steps Taken

### 1. Data Cleaning
- **Handling Missing Values**:
  - Filled missing `Age` values based on `Pclass` and `Sex`.
  - Imputed `Embarked` with the mode.
  - Removed rows with missing `Cabin` values.
  - Addressed a single missing value in `Fare` with the median.

- **Outlier Detection**:
  - Analyzed numerical features (`Fare` and `Age`) using boxplots.

### 2. Feature Engineering
- Created a `FamilySize` feature by combining `SibSp` and `Parch`.
- Converted the `Sex` column to binary (male: 0, female: 1).

### 3. Scaling
- Scaled `Age` and `Fare` using MinMaxScaler for normalization.

---

## Key Insights
- Certain Pclass groups had distinct age distributions, influencing survival rates.
- High variance in `Fare` values necessitated scaling for machine learning.

---

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/titanic-cleaning.git

