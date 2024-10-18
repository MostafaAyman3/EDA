# EDA on Adult Dataset

This repository contains exploratory data analysis (EDA) of the Adult dataset, which is used for predicting income based on various features of individuals. The analysis is performed using Python and libraries such as Pandas, NumPy, Matplotlib, and Seaborn.

## About the Adult Dataset

- **income (target)**: whether or not an individual makes more than $50,000 annually (<=50K, >50K).
- **age**: the age of an individual (Integer > 0).
- **workclass**: represents the employment status of an individual (e.g., Private, Self-emp-not-inc, etc.).
- **fnlwgt (final weight)**: number of people the census believes the entry represents.
- **education**: level of education achieved by an individual (e.g., Bachelors, HS-grad, etc.).
- **education-num**: level of education achieved in numerical form (Integer > 0).
- **marital-status**: marital status of an individual (e.g., Married-civ-spouse, Never-married, etc.).
- **occupation**: type of occupation of an individual (e.g., Tech-support, Exec-managerial, etc.).
- **relationship**: represents what this individual is relative to others (e.g., Husband, Wife, etc.).
- **race**: descriptions of an individual’s race (e.g., White, Black, etc.).
- **gender**: (Male, Female).
- **capital-gain**: capital gains for an individual (>= 0).
- **capital-loss**: capital loss for an individual (>= 0).
- **hours-per-week**: the hours an individual has reported to work per week (continuous).

## EDA Process

1. **Data Loading**:
    - Loaded the dataset using Pandas.
    - Checked for missing values and duplicates.

2. **Data Cleaning**:
    - Dropped rows with null values and removed duplicates.
    - Cleaned string columns to remove quotation marks and replaced `?` with NaN.

3. **Data Visualization**:
    - Created heatmaps and count plots to visualize correlations and distributions.
    - Analyzed the distribution of numerical features using box plots and histograms.
    - Visualized the representation of different races and education levels in the dataset.

4. **Feature Engineering**:
    - Dropped irrelevant features like `education` and `capital-gain`.
    - Encoded categorical features using Label Encoding.

5. **Analysis of Working Hours**:
    - Analyzed average working hours based on education level.
    - Visualized the balance of the target variable.

## Dependencies

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the directory:
   ```bash
   cd <directory-name>
   ```
3. Ensure you have the required libraries installed:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook:
   ```bash
   jupyter notebook EDA_adult_dataset.ipynb
   ```
