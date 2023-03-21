# Exploratory-Data-Analysis-Of-PPP-Loan-Data-using-Pyspark
## Introduction
The goal of this project is to perform exploratory data analysis on PPP loan data using PySpark. The Paycheck Protection Program (PPP) was a federal loan program in the United States that provided loans to small businesses affected by the COVID-19 pandemic. The loan data contains information such as loan amount, loan type, business name, address, and more.

In this project, we used PySpark to analyze the PPP loan data and answer various questions related to the loans. We started by loading the data into a PySpark dataframe, cleaning and preprocessing it.

To add more insights to the analysis, we also concatenated census data with the loan data based on the zip code of each loan. This will allow us to analyze the loan data in relation to various demographic and socio-economic characteristics of the zip codes.
## Analysis:
### 1. Top 10 Banks that Loaned Money
  ![image](https://user-images.githubusercontent.com/48169929/226631379-4576948e-4fbb-441b-b593-b08cdaef6e56.png)
* Among the Top 10 banks that loaned the most money, there are 3 banks in Ohio, 2 banks in Denver and 2 banks in North Carolina.
### 2. Top 10 Banks that loaned the Most Money to Businesses in the Same State
  ![image](https://user-images.githubusercontent.com/48169929/226632242-6218e8ca-1591-4161-b1f4-13169a96f9c1.png)
### 3. Top 10 Zip Codes with the Most Funding Per Capita
  ![image](https://user-images.githubusercontent.com/48169929/226632463-b2ad7d6f-15ba-48f9-b0e3-61e3d3c206db.png)
* We can see that among the Top 10 Zip Codes, 4 Zip Codes are in California, 3 are in Illinois and 2 are in New York.
### 4. Top Industries (NAICS codes) in the top 100 zip codes that received money
  ![image](https://user-images.githubusercontent.com/48169929/226636992-a5ae7948-cc6f-411e-b862-9892b851bf02.png)
### 5. Scatter Plot : Percentage of Population whose Income is below Poverty Level vs Loan Amount
  ![image](https://user-images.githubusercontent.com/48169929/226639406-7c41284a-7e9f-471a-a472-001fab9ec06e.png)
#### Percentage of Population whose Income is below Poverty Level vs Loan Amount (for Loan Amounts greater than 8 Million)
  ![image](https://user-images.githubusercontent.com/48169929/226639864-55b4954b-f728-45ce-b44e-1f948e8bd9e4.png)
* The scatter plots illustrate the relationship between loan amount and the percentage of population living below the poverty level in the top 100 zip codes.
* The first scatter plot includes all loan amounts, whereas the second scatter plot only includes loan amounts that are greater than 8 million.
* It can be observed that loan amounts exceeding 8 million are only approved for zip codes where the percentage of population with income below poverty level is less than 20%. In other words, loans greater than 8 million are granted only to zip codes where approximately 80% of the population has an income above the poverty level.
* There are two reasons why this finding is reasonable. Firstly, individuals with higher incomes are more likely to be able to make the monthly repayments on a large loan. 
* Secondly, banks conduct background and income checks before granting loans, so a high income is typically required to qualify for a larger loan amount.
*  As shown in the plots, zip codes with a higher percentage of population with income above poverty level are more likely to have residents with higher incomes, increasing their chances of being approved for larger loans.

  
