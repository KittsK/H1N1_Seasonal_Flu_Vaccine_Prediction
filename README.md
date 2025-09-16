#  H1N1 and Seasonal Flu Vaccine Uptake Prediction
---
## Overview of the Project
This project is aimed at understanding and predicting public uptake of the H1N1 and seasonal flu vaccines. Using data from the National 2009 H1N1 Flu Survey (NCFS), this project involves a complete data science lifecycle, from data cleaning and exploratory data analysis to predictive modeling and the generation of actionable insights for public health campaigns.
---
## Business Understanding
Influenza, a contagious respiratory illness, poses a significant public health threat annually through seasonal outbreaks and occasional pandemics like the 2009 H1N1 swine flu. Vaccination is the most effective preventative measure against influenza and its severe complications. Public health organizations, such as the Centers for Disease Control and Prevention (CDC), invest heavily in vaccination campaigns. The effectiveness of these campaigns hinges on public willingness to get vaccinated, known as "vaccine uptake". This project seeks to identify the key factors that drive vaccination decisions to help public health officials design more effective and targeted vaccination campaigns.
---
## Data Understanding
The dataset contains **26,707 rows** and **38 columns**.
* **Target Variables:** The two columns we aim to predict are `h1n1_vaccine` and `seasonal_vaccine`. Both are **binary**, where `1` means the respondent received the vaccine and `0` means they did not. This defines our task as a **binary classification problem**.
* **Data Types:** The dataset is a mix of numerical and categorical data.
    * **Numerical:** Many features are encoded as numbers (e.g., `h1n1_concern` from 0-3) which represent ordinal scales.
    * **Categorical:** Features like `age_group`, `race`, and `employment_status` are represented as strings and will require encoding for use in most machine learning models.
---
## Data Preparation
The data preparation phase involved several key steps to handle inconsistencies and prepare the data for modeling:

**Handling Missing Values:** Missing values in various columns were imputed. For categorical columns, the mode was used, while for numerical columns, the mean was used.
**Encoding Categorical Variables:** Categorical features were converted into a numerical format using one-hot encoding.
**Feature Engineering:** Some columns were transformed or combined to create new, more informative features.
---
## Methodology
1. **Business Understanding**: Define objectives 
2. **Data Understanding**: Explore data distribution, missing values, and correlations
3. **Data Preparation**: Cleaning, feature engineering, encoding
4. **EDA**:
   - Univariate, bivariate, and multivariate analysis
5. **Modeling**:
   - Logistic Regression, Random Forest, XGBoost
   - Hyperparameter tuning with GridSearchCV
6. **Evaluation**:
   - Performance measured with Accuracy, Precision, Recall, F1-score, ROC-AUC
   - Confusion matrices to evaluate misclassifications
---

## Visualizations

- Distribution of Target Variables
- Vaccination by Age Group
- Vaccination by Doctor's Recommendation
- H1N1 Concern vs. Vaccination
- Race and Vaccination
---

## Key Findings

- **Doctor's recommendation** is one of the most significant predictors of vaccination for both H1N1 and seasonal flu.
- **Health insurance coverage** is also a strong predictor, indicating that access to healthcare plays a crucial role in **vaccination decisions.**
- **Age** is a significant factor for the seasonal flu vaccine, with older individuals being more likely to get vaccinated.
- Opinion-based features, such as **concern about the flu** and **perceived effectiveness** and safety of the vaccine, are also highly influential.


 ## Recommendations

1. **Leverage Healthcare Providers:** Public health campaigns should focus on educating and encouraging healthcare providers to recommend flu vaccines to their patients.
2. **Address Vaccine Concerns:** Public health communications should proactively address common concerns about vaccine efficacy and safety 
3. **Multi-Channel Communication:** To reach a wider audience, public health agencies should use a variety of communication channels, including social media, traditional media, and community outreach programs
 
## Deliverables

- ✅ **Jupyter Notebook** with EDA, feature engineering, and model building
- ✅ **Cleaned dataset** for analysis
- ✅ **Presentation slides** for stakeholders
- ✅ **README.md** (this file)


## Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn, XGBoost
- Jupyter Notebook
- CRISP-DM methodology
