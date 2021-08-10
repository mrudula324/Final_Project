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
5. Feature Engineering
   -
5. One hot encoding and Label encoding
6. Outliers removal
7. Univariate analysis for important variables
8. Bivariate analysis to understand relation between variables
9. Multivariate analysis for identify the hightly correlated independent variables
10. Machine Leaning modeling:
  We used supervised learning models to predict the chargedoff borrowers.
  Models Used:
     - Logistic Regression
     - Random Forest
     - KNN
     - XgBoost
     
  We ran models with various resampling methods, as the data set is found to be biased. 
      - Imbalanced dataset
      - SMOTENN
      - SelectKBEST
     
  roc,roc-auc curves were plotted for all the methods.
10. Model scores were tabulated for comparision.

![image](https://user-images.githubusercontent.com/79874273/128814414-372a0cc8-bd5b-4d64-b3c0-83e65581e4b1.png)


***
# Results:

***
 
