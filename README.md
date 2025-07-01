# Python-Project-EDA
Exploratory Data Analysis on Titanic dataset

This project involves a detailed Exploratory Data Analysis (EDA) on the Titanic dataset to understand passenger demographics, relationships between variables, and key factors influencing survival. The analysis is performed using Python and various data science libraries like pandas, matplotlib, and seaborn.

✅ Steps Followed:
1. Data Loading
Imported Titanic dataset using pandas.
Inspected basic structure, data types, and initial shape.

2. Data Cleaning
Handled missing values:
Filled missing Age with median.
Filled missing Embarked with mode.
Dropped the Cabin column due to high missingness.

3. Data Overview
Used df.info(), df.describe(), and .value_counts() to understand dataset structure and value distribution.

4. Data Type Conversion
Converted categorical and numerical columns to appropriate data types for analysis.

5. Univariate Analysis
Explored individual columns:
Histograms, boxplots, and KDE plots for numerical features (Age, Fare).
Count plots for categorical features (Sex, Embarked, Pclass, Survived).
Identified distributions and outliers.

6. Bivariate Analysis
Explored relationships between variables:
Survival rates by Sex, Pclass, Embarked, etc.
Used groupby, barplot, and cross-tabulation.

7. Correlation Analysis
Created a correlation heatmap of numerical features using sns.heatmap().
Identified moderate correlation between Fare and Survived.

8. Feature Engineering
Created new features to enhance predictive potential:
Title Extraction from passenger names.
FamilySize and IsAlone to represent travel group size.
AgeGroup (Child, Teen, etc.) via pd.cut().
FareGroup via pd.qcut() for fare-based segmentation.
Fare_per_Person for normalizing group ticket fares.
Deck extracted from cabin data (optional).
Encoded categorical variables for potential use in modeling.

📊 Tools & Technologies Used
Languages: Python
Libraries: pandas, seaborn, matplotlib, numpy
Platform: Jupyter Notebook
