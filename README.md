# Lending Club Peer-to-Peer Data Analysis:
***
# Introduction:
Lending Club is the USA largest electronic peer-to-peer lending platform. Lending club has less overhead costs compared to traditional banks. Therefore, this has been a huge sucesses in past years. Lending club offers loans starting from 5000 to a max of 40000. Borrowers fill out a loan application that includes his personal details, credit and delinq records and loan amount they are requesting and term that they repay loan in full. Though lending club moniters various factors to approve loan to the borrower there are some cases the loans has been charged off. Analysis has been done using machine learning models to identify the credibility of the borrower and to minimize defaulters.

***
# Data Analysis:
1. Checked for basic statistics of the data.
   - Basic functions such as describe, shape,check for nulls has been performed. 
   - Target variable is bivariate, constains "0" for charged off and "1" for fully paid. 
2. Preprocessing 
   - Droped unwanted columns that are not in the scope of our analysis.
   - Droped columns with more than 50% of nulls.
   - Removed columns that has unique values.
3. Output from step 2 is used for ETL Processing.
   - Aure postgress database is created and stored with appropriate data.
   - Using psycopg2 conection has been established to Azure server.
   - Created dataframes for tables and inserted tables along with the data into the azure postgress.
   - documentation can be found in week24_final_project_ETL.ipynb.
   - Now azure is connected ready to use and can connected to query records any time.
   - We also connected postgress to local host.
4. Feature Engineering
   - Some new columns were created by extracing data from the original columns. ex: month from earliest_cr_line and value from term.
   - States has been categorized based on the regions.
5. One hot encoding for all nominal columns and Label encoding for ordinal variables. 
6. Outliers has been observed on box plots and thus removed them based on z-scores.
7. Univariate analysis for specific variables to understand their distribution.
8. Bivariate analysis, plots were done to understand relation between variables and observations were documented.
9. Multivariate analysis for identify the hightly correlated independent variables.
10. Heatmap is created to anlyze the correlation between all independent variables. 
11. Pandas profiler is executed to understand the eda view from pandas. 
12. Feature Selection 
   - RFE with logistic regression is executed to get the understand f
   - SelectKBest, Method from sklearn library is also used for feature rankings. 
13. Created funcations for model evaluations, roc and roc-auc plotting. 
14. On step 1 we understood that dataset is imbalanced therefore, we tried following resampling methods for the all the models.
   - Imbalanced dataset: use data as it is for modeling.
   - SMOTENN - Method from imblearn library for resampling.
   - We also tried manual sampling the same number of records as minority class and perfomed modeling. But results turned out be undesirable. 
15. Supervised machine leaning modeling:
   - Logistic Regression
   - Random Forest
   - KNN
   - XgBoost
   - LDA roc,roc-auc curves were plotted for all the methods.

16. Model scores were tabulated for comparision.

![image](https://user-images.githubusercontent.com/79874273/128814414-372a0cc8-bd5b-4d64-b3c0-83e65581e4b1.png)


***
# Results:

***
 
