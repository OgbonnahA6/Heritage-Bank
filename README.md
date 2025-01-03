# HERITAGE BANK LOANS ANALYSIS
---
![BankImage](https://github.com/user-attachments/assets/ab4cba37-ed71-4cd6-97f5-bcfcdc56e41a)

---
### A. Overview: 
The analysis focused on understanding key factors that impact loan performance, particularly identifying predictors of loan defaults. The dataset contained borrower information, loan characteristics, and repayment details, allowing for an in-depth examination of risk indicators. 
#### Key Objectives:
- Identify Default Risk Factors: Pinpoint the primary variables driving loan defaults.
- Analyze Borrower Characteristics: Investigate how borrower attributes such as income, debt-to-income ratio (DTI), and employment length influence loan outcomes.
- Examine Feature Relationships: Evaluate the interactions between key loan variables, including loan amount and interest rate, and their effect on default risk.
- The analysis leverages SQL for advanced data processing and Power BI for insightful visualizations, delivering actionable insights into loan repayment trends, default probabilities, and customer segmentation. By integrating data-driven decision-making into its operations, the bank can optimize lending practices, improve risk management, and enhance financial performance.
---
### B. Problem Statement: 
The bank aims to enhance its lending operations by creating a comprehensive, actionable loan analysis report. This report will evaluate key loan performance metrics, identify default risk factors, and uncover trends in borrower behavior. Leveraging advanced data analytics and visualization techniques, the analysis seeks to optimize loan portfolio management, improve risk assessment, and support data-driven decision-making. Key focus areas include tracking loan application trends, benchmarking loan quality, and segmenting borrowers based on risk profiles to ensure strategic and sustainable growth.
---
### C. Data Collection and Processing: 
- Banks gather loan data from various sources, including loan applications, credit reports, income verification processes, collateral evaluations, and digital platforms.
- The dataset used in this analysis, **Loan_financial**, includes key attributes of loan applicants such as credit score, income, employment length, loan amount, and loan status.
---
### D. Data Set Descriptions:
- The dataset contains several columns with detailed information about loan applicants and their loan details. Here's a breakdown of key columns to help guide the analysis:

#### 1. Borrower Characteristics:
  - address_state: The state of residence.
  - application_type: Whether the loan is for an individual or joint application.
  - emp_length: Employment length of the borrower.
  - emp_title: Job title of the borrower.
  - annual_income: Borrower's annual income.

#### 2.	Loan Characteristics:
  - grade: Loan grade assigned based on credit risk.
  - sub_grade: More granular classification of loan risk.
  - term: Duration of the loan (36 or 60 months).
  - int_rate: the interest rate of the loan.
  - loan_amount: Principal loan amount.
  - installment: Monthly payment required.
  - verification_status: Whether the borrower's income has been verified.

#### 3.	Payment and Credit Metrics:
  - total_acc: Total number of credit accounts.
  - dti: Debt-to-income ratio.
  - total_payment: Total amount paid towards the loan so far.
  - last_payment_date and last_credit_pull_date: Dates related to payments and credit checks.
---
### E. Exploratory Data Analysis (EDA): 
#### Summary of Insights
#### 1. Amount Distribution
  - Loan amounts exhibited a right-skewed distribution, with a concentration of smaller loans and fewer larger facilities. This aligns with bank lending practices, whereby a majority of borrowers prefer smaller loans.

#### 2. Interest Rate Distribution
- Interest rates cluster around common values and increase progressively for riskier loans. Borrowers with higher risk profiles, such as those with lower credit scores, are generally charged higher interest rates.

#### 3. Annual Income Distribution
- Annual income spans a broad range with potential outliers, reflecting a diverse borrower population. This variability likely influences both loan approval and repayment capabilities.

#### 4. Debt-to-Income Ratio (DTI) Distribution
- Borrowers with higher DTI ratios tend to have greater financial commitments relative to their income, posing a higher risk of default. This risk is amplified when combined with lower incomes and higher interest rates.

#### 5. Correlation Insights
##### 5.1 Loan Amount vs. Interest Rate:
  - A moderate positive correlation indicates that larger loans are associated with higher interest rates, likely reflecting the increased risk.
##### 5.2 Annual Income vs. Loan Amount:
  - Higher-income borrowers tend to secure larger loans, demonstrating a positive relationship.
##### 5.3 DTI vs. Interest Rate:**
  -  Borrowers with higher DTI ratios are often charged higher interest rates, as lenders perceive them as riskier due to existing debt obligations.

### F. Key Takeaways
##### 1. Risk Indicators
  -  Higher loan amounts, elevated interest rates, and increased DTI ratios are key indicators of potential default risk. Borrowers with lower incomes and higher DTIs should be evaluated with stricter approval criteria or offered alternative repayment structures.

##### 2. Segmentation Potential:
  - Segmenting borrowers by income, loan amount, and interest rate enables more precise risk assessment and supports the optimization of lending strategies.

##### 3. Feature Relationships:
  - Understanding correlations between key features such as income, loan amount, and interest rates provides actionable insights for building predictive models to identify default risks and improve lending practices.
---
### G. Methodology: 
The methodology for this loan analysis project employed advanced data analysis techniques and strategic planning to deliver actionable insights:
#### 1. Correlation Analysis:
- Conducted a correlation analysis to uncover relationships between key factors such as loan amount, interest rates, borrower income, and loan default risk. This helped identify high-risk borrower segments and key indicators of potential defaults.
#### 2. Market Benchmarking:
- Benchmarked loan portfolio performance against industry standards and peer institutions, evaluating metrics such as default rates, interest rate structures, and portfolio growth to gauge competitiveness and identify areas for improvement.
#### 3. Data Visualization:
- Utilized advanced visualization techniques to analyze loan performance trends. Charts and graphs provided comparative insights into loan risk profiles, repayment behaviors, and portfolio diversification, enabling a clearer understanding of performance metrics and risk management strategies.
#### 4. Dashboards:
  1. Summary Dashboard
  2. Overview Dashboard
  3. Details Dashboard
---
### H. SQL Query Codes

  Query 1                                                                                |               Query 2
:--------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------:
![SQL1](https://github.com/user-attachments/assets/f1c67c0d-65e5-49fe-ae5f-048303629a8e) |  ![SQL2](https://github.com/user-attachments/assets/7a8211d9-aa24-458c-90cb-6fe1982a28ca)

  Query 3                                                                                |               Query 4
:--------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------:
 ![SQL3](https://github.com/user-attachments/assets/e6885be4-1c04-4a02-94c2-e74329062f19)|  ![SQL4](https://github.com/user-attachments/assets/e30d6c95-273e-40d9-8bf9-503d4431fbfd)

  Query 5                                                                                |               Query 6
:--------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------:
![SQL5](https://github.com/user-attachments/assets/a559b93a-0cab-47ce-848a-66f88dbdc27c) |  ![SQL6](https://github.com/user-attachments/assets/663d3f14-82e9-4c3d-847e-cbeef7d51edd)

  Query 7                                                                                |               Query 8
:--------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------:
![SQL7](https://github.com/user-attachments/assets/e225cc3b-1c70-4ead-99cc-23436343b064) | ![SQL8](https://github.com/user-attachments/assets/7ef41e84-e566-43c4-afd3-9d040ef90dcd)

  Query 9                                                                                              
:--------------------------------------------------------------------------------------: 
![SQL9](https://github.com/user-attachments/assets/2389838a-4a9d-4320-a65d-812882b79725)  

---
### I. Results: 
The analysis yielded several significant findings:
#### 1. Risk Assessment:
##### Loan Grades and Defaults
##### Insight:
  - Higher loan grades (like A or B) tend to be associated with lower interest rates and smaller loan amounts, while lower grades (C, D, E) have higher interest rates and larger loans.
  - Additionally, loans with lower grades show higher total payments, which could imply a higher repayment burden due to interest accumulation.
##### Recommendation
  - Focus on refining loan approval criteria for applicants in lower-grade categories.
  - Consider implementing additional support mechanisms (e.g., financial counseling or better structuring of repayment plans) to reduce default risk in these groups.
  
#### 2. Borrower Financial Health and Loan Performance
##### Insight
  - Borrowers with longer employment histories and higher annual incomes tend to make higher total payments, indicating better loan performance. This suggests that stable employment is a key indicator of financial health and repayment ability.
##### Recommendation
  - Prioritize borrowers with longer employment lengths and higher incomes in loan approvals.
  - Consider offering preferential terms (lower interest rates) to these demographics, as they exhibit lower risk.
---
#### 3. Summary Dashboard:
  ![Slide1](https://github.com/user-attachments/assets/7cb5fa27-ecf5-4e98-b24b-89a3d080bd32)

#### 4. Debt-to-Income Ratio (DTI) Analysis
##### Insight
  - The debt-to-income ratio (DTI) has a weak positive correlation with both loan amount and total payments, meaning that while a higher DTI may slightly increase loan size, it does not significantly impact repayment.
  - This also indicates that higher DTI does not strongly correlate with an increased risk of repayment issues.
##### Recommendation
  - DTI should still be considered an important part of the overall risk assessment, but it may not need to be heavily weighted.
  - Focus more on factors like income stability and loan grade when determining default risk.
  
#### 5. Loan Amount vs Interest Rate Trends
##### Insight
  - A moderate positive correlation between loan amount and interest rates, meaning larger loans tend to come with higher interest rates. This could be because larger loans are perceived as riskier, requiring a higher return.
##### Recommendation:
  - Monitor larger loan segments for repayment challenges. Explore offering improved terms, such as reduced interest rates or extended repayment periods, specifically targeting higher-income individuals to enhance repayment rates on larger loans.
---
#### 6. Overview Dashboard
![Slide2](https://github.com/user-attachments/assets/31e4d74f-a693-473f-800c-7288c8973400)

#### 7. Geographical Trends
##### Insight
- States differ significantly in average loan amounts, interest rates, and repayment performance. Some states show higher average loan amounts with lower repayments, indicating potential regional economic or demographic challenges.
##### Recommendation
- Tailor loan products based on regional data. Consider adjusting lending criteria, interest rates, or loan caps for states with poorer loan performance. Offering regional promotions or financial education programs could also improve repayment behavior.
---
#### 8. Details Dashboard:
![Slide3](https://github.com/user-attachments/assets/16790c9c-32b2-4f7d-9c1f-37c603a312ca)

### J. Recommendations: 
##### 1. Stricter Loan Approval for High-Risk Loans:
- Borrowers with lower incomes and high debt-to-income ratios should be subjected to stricter loan approval criteria. This could include verifying the borrower’s financial health more thoroughly or offering smaller loan amounts to reduce default risk.
##### 2. Adjust Interest Rates for Riskier Borrowers:
- Since higher interest rates are associated with default, the lending institution may want to reconsider its pricing strategy. Offering more competitive rates to lower-risk borrowers could enhance repayment performance.
##### 3. Employment and Income Verification:
- Employment length and income are key predictors of loan performance. Focus on borrowers with stable, long-term employment when offering larger loans, or tailor repayment plans to align with their employment stability.
##### 4. Focus on Large Loan Monitoring:
- Larger loans are more prone to default and to reduce default rates, closer monitoring or more structured repayment options might be required.
#### 5. Overall Strategic Recommendations:
- **Enhanced Credit Risk Modeling**: Consider incorporating more advanced predictive models (e.g., machine learning) to assess the likelihood of defaults based on loan grades, borrower characteristics, and geographical factors.
- **Custom Loan Terms**: Offer tailored loan products with flexible interest rates and terms based on borrower stability (income, employment length) and regional characteristics.
- **Focus on High-Employment Borrowers**: Given the strong correlation between employment length and better repayment, focus lending efforts on individuals with more stable employment.
- **Regional Strategy**: Develop a regional strategy that adjusts lending terms based on state-specific performance, addressing areas where loan performance is subpar.
---
### K. Future Work: 
- Heritage Bank to focus on the following key areas of loan analysis for future work to enhance decision-making, risk management, and portfolio performance:
##### 1. Predictive Modeling for Default Risk:
- Refine predictive models for loan default risk using machine learning techniques like Random Forest, Gradient Boosting, or Neural Networks. Enhance accuracy by incorporating additional data, including borrower characteristics, macroeconomic indicators, and behavioral patterns.
##### 2. Customer Segmentation and Personalized Lending:
- Conduct customer segmentation analysis to understand borrower profiles and tailor lending products accordingly. Segmentation based on income, credit history, and repayment behavior can help design more personalized loan terms, reducing default risk and increasing customer satisfaction.
##### 3. Portfolio Stress Testing:
- Implement stress testing models to evaluate how external factors (e.g., economic downturns, interest rate hikes, regulatory changes) impact loan portfolio performance. This will help identify vulnerabilities and prepare the institution for adverse economic scenarios.

---
### L. Conclusion:
#### Summary of key findings
  - Defaulted loans have a higher average loan amount **($12,635)** than non-defaulted loans **($11,202)**, indicating that borrowers with larger loans may face an increased risk of default.
  - The average interest rate for defaulted loans is higher **(13.89%)** than for non-defaulted loans **(11.92%)**, suggesting that higher-risk loans with elevated interest rates are more prone to default.
  - Borrowers who default typically have a lower average income **($62,420)** than non-defaulted borrowers **($70,151)**, implying that lower income levels may hinder repayment ability.
  - The debt-to-income ratio is slightly higher for defaulted loans **(14.13%)** than non-defaulted loans **(13.27%)**, indicating that a higher debt burden relative to income increases the likelihood of default.
  - Defaulted loans are often associated with borrowers with shorter employment histories, potentially reflecting reduced financial stability. This trend aligns with income data, highlighting that less stable employment may correlate with diminished repayment capacity.

- The Heritage Bank loan analysis highlights key insights into loan performance, customer behavior, and risk management, emphasizing the value of data-driven decision-making to optimize lending practices, reduce risks, and enhance financial outcomes.
---


**MY APPRECIATION TO DATA TUTORIALS FOR PROVIDING THE DATASET AND GUIDANCE IN DOING THIS PROJECT.
