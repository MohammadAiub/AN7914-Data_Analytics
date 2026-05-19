
# AN7914: Lending Club Interest Rate Analysis

## Overview
This project analyzes the determinants of interest rates in the consumer credit market using data from Lending Club, a peer-to-peer lending platform. The objective is to identify key borrower characteristics that influence pricing through exploratory data analysis (EDA) and multiple linear regression modeling.

## Dataset
The dataset  `loans_dataset.csv` contains 10,000 rows from Lending Club, a peer-to-peer lending platform, with each row representing a unique consumer loan. It contains borrower characteristics (e.g., income, employment length, credit history) and loan-specific details (e.g., amount, term, grade) used to analyze the determinants of interest rates in the consumer credit market.

## Project Structure
- `analysis.ipynb`: Jupyter Notebook containing all data cleaning, EDA, feature engineering, and regression modeling code.

## Methodology
1. **Data Preparation:** Subsetting variables, handling missing values, and renaming columns for clarity.
2. **Exploratory Data Analysis (EDA):** Descriptive statistics and visualizations (histograms, scatterplots, boxplots) to understand distributions and relationships.
3. **Feature Engineering:** Creation of derived variables:
   - `credit_util`: Credit utilization ratio.
   - `bankruptcy_dummy`: Binary indicator for public bankruptcy records.
4. **Regression Modeling:** Five OLS models were fitted to assess the impact of risk factors on interest rates:
   - Model 1: Simple Linear Regression (Debt-to-Income)
   - Model 2: Simple Linear Regression (Bankruptcy)
   - Model 3: Categorical Regression (Income Verification)
   - Model 4: Multiple Regression (Credit Risk Controls)
   - Model 5: Full Specification with all controls (Grade, Term, Homeownership, etc.)

## Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AN7914-LendingClub-Analysis.git
   cd AN7914-LendingClub-Analysis


2. Run the Notebook:
   ```bash
   jupyter notebook analysis.ipynb
   ```
   
