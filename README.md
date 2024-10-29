# HERITAGE BANK LOANS ANALYSIS

![image](https://github.com/user-attachments/assets/85388c10-abe4-4bc5-85df-c66d2f83805d)

### Overview: 
The analysis focused on understanding key factors that impact loan performance, particularly identifying predictors of loan defaults. The dataset contained borrower information, loan characteristics, and repayment details, allowing for an in-depth examination of risk indicators. The key objectives were:
1.	**Identify Default Risk Factors**: Determine the primary variables contributing to loan defaults.
2.	**Analyze Borrower Characteristics**: Examine the relationship between borrower traits (income, DTI, employment length) and loan outcomes.
3.	**Explore Feature Relationships**: Assess the interplay between key loan variables like loan amount, interest rate, and their impact on default risk.
Utilizing SQL for sophisticated data processing and Power BI for advanced visualization, the analysis is designed to provide actionable intelligence on loan repayment trends, default probabilities, and customer segmentation. By embedding data-driven decision-making into operational strategies, the bank can refine its lending practices, effectively manage risk, and significantly enhance overall financial performance.

### Background: 
Analyzing loan data is essential for banks, enhancing several critical aspects of their operations. 
- First, it bolsters risk management by providing valuable insights into potential default risks and loan performance, enabling banks to implement proactive measures and effectively manage their risk exposure. 
- Second, it facilitates informed decision-making by delivering data-driven insights into loan portfolios, thereby supporting more strategic planning and targeted interventions. 
- Furthermore, performance monitoring is significantly optimized, as banks can track various metrics related to loan repayment and portfolio health, identifying trends and areas for improvement.
- Additionally, loan data analysis plays a pivotal role in fraud detection by uncovering anomalies and patterns indicative of fraudulent activity, thus protecting the institution’s assets. 
- Lastly, it offers invaluable customer insights, enabling banks to better understand borrower behavior and preferences, and enhancing customer relationship management. It also allows for tailoring of financial products to more effectively meet customer needs.

### Data Collection and Processing: 
Banks gather loan data through multiple channels, including loan applications, credit reports, income verification processes, collateral assessments, and digital platforms. The dataset (Loan_financial) used in this analysis contains information about loan applicants, including attributes such as credit score, income, employment length, loan amount, and loan status.

### Data Set Descriptions:
The dataset contains several columns that provide detailed information about loan applicants and their loan details. Here's a breakdown of key columns to help guide the analysis:

1.	**Borrower Characteristics:**
  a. address_state: The state of residence.
  b. application_type: Whether the loan is for an individual or joint application.
  c. emp_length: Employment length of the borrower.
  d. emp_title: Job title of the borrower.
  e. annual_income: Borrower's annual income.

2.	**Loan Characteristics:**
  f. grade: Loan grade assigned based on credit risk.
  g. sub_grade: More granular classification of loan risk.
  h. term: Duration of the loan (36 or 60 months).
  i. int_rate: the interest rate of the loan.
  j. loan_amount: Principal loan amount.
  k. installment: Monthly payment required.
  l. verification_status: Whether the borrower's income has been verified.

3.	**Payment and Credit Metrics**:
  m. total_acc: Total number of credit accounts.
  n. dti: Debt-to-income ratio.
  o. total_payment: Total amount paid towards the loan so far.
  p. last_payment_date and last_credit_pull_date: Dates related to payments and credit checks.

### Exploratory Data Analysis (EDA): 


  #### Summary of EDA Analysis Insights:
1.	**Loan Amount Distribution**:
  Loan amounts likely exhibit a right-skewed distribution, with a concentration of smaller loans and fewer larger loans. This suggests a typical lending practice where more borrowers take out smaller loans.
2.	**Interest Rate Distribution**:
  Interest rates likely cluster around common values, with a gradual increase for riskier loans. Borrowers with higher risk profiles (e.g., lower credit scores) are typically charged higher interest rates.
3.	**Annual Income Distribution**:
  Annual income is expected to span a broad range, with potential outliers on both ends. This indicates that the dataset covers a diverse population of borrowers with different income levels, potentially influencing loan approval and repayment ability.
4.	**Debt-to-Income Ratio (DTI) Distribution**:
  A higher debt-to-income ratio could signal borrowers with greater financial commitments relative to their income. These borrowers may pose a higher risk, especially when combined with lower income and higher interest rates.
5.	**Correlation Insights**:
  a. **Loan Amount vs. Interest Rate:** Likely a moderate positive correlation, meaning larger loans tend to have higher interest rates due to perceived higher risk.
  b. **Annual Income vs. Loan Amount:** Higher-income borrowers may take out larger loans, showing a positive relationship.
  c. **DTI vs. Interest Rate:** Borrowers with higher DTI ratios could be charged higher interest rates, as lenders may view them as riskier due to their existing debt burden.

**Key Takeaways**:
  a. **Risk Indicators:** Higher loan amounts, interest rates, and DTI ratios are all potential indicators of higher loan default risk. Borrowers with lower incomes and higher DTIs should be considered for stricter approval criteria or different repayment structures.
  b. **Segmentation Potential:** Segmenting borrowers by income, loan amount, and interest rate can provide deeper insights into specific risk groups and optimize lending strategies.
  c. **Feature Relationships:** Understanding the correlations between income, loan amount, and interest rates helps identify patterns that could guide predictive modeling for loan defaults.

### Methodology: 
The methodology applied in this loan analysis project integrated a range of advanced data analysis techniques and strategic planning approaches:
•	**Correlation Analysis**: We performed correlation analyses to identify relationships between key factors such as loan amount, interest rates, borrower income, and loan default risk, with particular emphasis on identifying high-risk borrower segments and potential default indicators.
•	**Market Benchmarking**: The performance of the loan portfolio was benchmarked against industry standards, including comparisons to peer institutions, using metrics such as default rates, interest rate structures, and portfolio growth.
•	**Data Visualization Tools**: Advanced visualization techniques were employed to map loan performance trends over time. Various types of charts were utilized to provide comparative assessments of loan risk profiles, repayment behavior, and portfolio diversification, facilitating a deeper understanding of performance metrics and risk management strategies.

### Results: 
The analysis yielded several significant findings:
#### Risk Assessment: Loan Grades and Defaults
•	**Insight**: Higher loan grades (like A or B) tend to be associated with lower interest rates and smaller loan amounts, while lower grades (C, D, E) have higher interest rates and larger loans. Additionally, loans with lower grades show higher total payments, which could imply a higher repayment burden due to interest accumulation.
•	**Recommendation**: Focus on refining loan approval criteria for applicants in lower-grade categories. Consider implementing additional support mechanisms (e.g., financial counseling or better structuring of repayment plans) to reduce default risk in these groups.
#### Borrower Financial Health and Loan Performance
•	**Insight**: Borrowers with longer employment histories and higher annual incomes tend to make higher total payments, indicating better loan performance. This suggests that stable employment is a key indicator of financial health and repayment ability.
•	**Recommendation**: Prioritize borrowers with longer employment lengths and higher incomes in loan approvals. Consider offering preferential terms (lower interest rates) for this demographic, as they exhibit lower risk.

#### Summary Dashboard:
  ![Slide1](https://github.com/user-attachments/assets/7cb5fa27-ecf5-4e98-b24b-89a3d080bd32)


#### Debt-to-Income Ratio (DTI) Analysis
**Insight**: The debt-to-income ratio (DTI) has a weak positive correlation with both loan amount and total payments, meaning that while a higher DTI may slightly increase loan size, it does not significantly impact repayment. This indicates that higher DTI does not strongly correlate with an increased risk of repayment issues.
**Recommendation**: DTI should still be considered an important part of the overall risk assessment, but it may not need to be heavily weighted. Focus more on factors like income stability and loan grade when determining risk.
  #### Loan Amount vs Interest Rate Trends
**Insight**: There is a moderate positive correlation between loan amount and interest rates, meaning larger loans tend to come with higher interest rates. This could be because larger loans are perceived as riskier, requiring a higher return.
**Recommendation**: Monitor larger loan segments for repayment issues. Consider offering better terms (such as lower interest rates or extended repayment periods) for higher-income individuals to improve repayment rates on larger loans.

#### Overview Dashboard
![Slide2](https://github.com/user-attachments/assets/31e4d74f-a693-473f-800c-7288c8973400)

  #### Geographical Trends
**Insight**: States differ significantly in average loan amounts, interest rates, and repayment performance. Some states show higher average loan amounts with lower repayments, indicating potential regional economic or demographic challenges.
**Recommendation**: Tailor loan products based on regional data. For states with poorer loan performance, consider adjusting lending criteria, interest rates, or loan caps. Offering regional promotions or financial education programs could also improve repayment behavior.

#### Details Dashboard:
![Slide3](https://github.com/user-attachments/assets/16790c9c-32b2-4f7d-9c1f-37c603a312ca)

### Recommendations: 
#### 1. Stricter Loan Approval for High-Risk Loans:
Borrowers with lower incomes and high debt-to-income ratios should be subjected to stricter loan approval criteria. This could include verifying the borrower’s financial health more thoroughly or offering smaller loan amounts to reduce default risk.
#### 2. Adjust Interest Rates for Riskier Borrowers:
Since higher interest rates are associated with default, the lending institution may want to reconsider its pricing strategy. Offering more competitive rates to lower-risk borrowers could enhance repayment performance.
#### 3. Employment and Income Verification:
Employment length and income appear to be significant indicators of loan performance. Consider focusing on borrowers with stable, long-term employment when offering larger loans, or offer repayment plans adjusted to employment stability.
#### 4. Focus on Large Loan Monitoring:
Larger loans are more prone to default. This might require closer monitoring or more structured repayment options for loans over a certain threshold to reduce default rates.

#### Overall Strategic Recommendations:
1.	**Enhanced Credit Risk Modeling**: Consider incorporating more advanced predictive models (e.g., machine learning) to assess the likelihood of defaults based on loan grades, borrower characteristics, and geographical factors.
2.	**Custom Loan Terms**: Offer tailored loan products with flexible interest rates and terms based on borrower stability (income, employment length) and regional characteristics.
3.	**Focus on High-Employment Borrowers**: Given the strong correlation between employment length and better repayment, focus lending efforts on individuals with more stable employment.
4.	**Regional Strategy**: Develop a regional strategy that adjusts lending terms based on state-specific performance, addressing areas where loan performance is subpar.

### Future Work: 
I recommended Heritage Bank to focus on the following key areas of loan analysis for future work to enhance decision-making, risk management, and portfolio performance:
  #### 1. Predictive Modeling for Default Risk:
•	Develop and refine predictive models using machine learning techniques such as Random Forest, Gradient Boosting, or Neural Networks to accurately forecast loan defaults. Incorporating additional borrower characteristics, macroeconomic factors, and behavioral data will improve the accuracy of default risk predictions.
  #### 2. Customer Segmentation and Personalized Lending:
•	Conduct customer segmentation analysis to better understand borrower profiles and tailor lending products accordingly. Segmentation based on income, credit history, and repayment behavior can help design more personalized loan terms, thereby reducing default risk and increasing customer satisfaction.
  #### 3. Portfolio Stress Testing:
•	Implement stress testing models to evaluate how external factors (e.g., economic downturns, interest rate hikes, regulatory changes) impact loan portfolio performance. This will help identify vulnerabilities and prepare the institution for adverse economic scenarios.
  #### 4. Fraud Detection and Anomaly Analysis:
•	Develop more advanced fraud detection algorithms by leveraging anomaly detection techniques and machine learning. Future work should focus on real-time monitoring systems that can identify fraudulent activities or irregularities in loan applications and repayment patterns.
  #### 5. Impact of Economic Indicators on Loan Performance:
•	Analyze the impact of key economic indicators such as inflation, unemployment rates, and GDP growth on loan repayment behavior and portfolio performance. This analysis can help institutions adjust their lending strategies in response to macroeconomic conditions.
  #### 6. Loan Product Innovation and Profitability Analysis:
•	Evaluate the profitability of different loan products by analyzing interest rates, loan durations, and borrower risk profiles. Future work should involve developing innovative loan products that cater to emerging market segments while maintaining a balance between profitability and risk.
Focusing on these areas will not only strengthen risk mitigation strategies but also enhance overall portfolio management and operational efficiency.

### Conclusion:
#### Summary of key findings:
1. Default loans have a higher average loan amount ($12,635) compared to non-defaulted loans ($11,202). This suggests that borrowers with larger loans may be at a higher risk of defaulting.
2. The average interest rate for defaulted loans is higher (13.89%) than for non-defaulted loans (11.92%). This indicates that riskier loans (with higher interest rates) are more likely to default.
3. Borrowers who default tend to have a lower average income ($62,420) compared to non-defaulted borrowers ($70,151). Lower income may contribute to the inability to meet repayment obligations.
4. The debt-to-income ratio is slightly higher for defaulted loans (14.13%) compared to non-defaulted loans (13.27%). This suggests that borrowers with a higher debt burden relative to their income are more likely to default.
5. Defaulted loans are associated with a smaller number of borrowers, which may imply that people with shorter employment histories are more prone to default. This is especially evident when combined with the income data, as less stable employment may correlate with lower repayment ability.
The Heritage Bank loan analysis provides a concise yet comprehensive evaluation of loan portfolio performance, customer behavior, and risk management. Leveraging SQL for efficient data processing and Power BI for dynamic visualizations, the analysis delivers actionable insights into loan repayment trends, default probabilities, and customer segmentation. By incorporating data-driven decision-making into its operational strategies, the bank can optimize lending practices, mitigate risks more effectively, and improve overall financial performance.



**MY APPRECIATION TO DATA TUTORIALS FOR PROVIDING THE DATASET AND GUIDANCE IN DOING THIS PROJECT.
