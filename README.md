# Lending Club Peer-to-Peer Data Analysis:
***
## Introduction:
Lending Club is the USA largest electronic peer-to-peer lending platform. Lending club has less overhead costs compared to traditional banks. Therefore, this has been a huge sucesses in past years. Lending club offers loans starting from 5000 to a max of 40000. Borrowers fill out a loan application that includes his personal details, credit and delinq records and loan amount they are requesting and term that they repay loan in full. Though lending club moniters various factors to approve loan to the borrower there are some cases the loans has been charged off. Analysis has been done using machine learning models to identify the credibility of the borrower and to minimize defaulters.

***
# Data Analysis:
1. Checked for basic statistics of the data.
2. Preprocessing 
   - Droped unwanted columns
   - Droped columns with more than 50% of nulls
   - Removed columns that has unique values
3. Feature Engineering
4. One hot encoding and Label encoding
5. Outliers removal
6. Univariate analysis for important variables
7. Bivariate analysis to understand relation between variables
8. Multivariate analysis for identify the hightly correlated independent variables
9. Machine Leaning modeling:
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
#Results:

***
 
