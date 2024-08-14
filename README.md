# BANK LOANS ANALYSIS



### Overview

This project is dedicated to the analysis of bank loan data with the objective of deriving comprehensive insights into loan portfolio performance, customer behavior, and risk assessment. Utilizing SQL for sophisticated data processing and Power BI for advanced visualization, the analysis is designed to provide actionable intelligence on loan repayment trends, default probabilities, and customer segmentation. By embedding data-driven decision-making into operational strategies, the bank can refine its lending practices, effectively manage risk, and significantly enhance overall financial performance.

### Bank Loan Domain Knowledge
Bank loan domain knowledge encompasses a comprehensive understanding of the various aspects of loan management, including loan types, underwriting processes, risk assessment, and regulatory compliance. This knowledge includes familiarity with loan products such as personal, mortgage, auto, and business loans, as well as the criteria for approving and managing these loans. It involves an understanding of credit scoring, interest rates, repayment schedules, and default management. Proficiency in this domain also requires insight into the financial metrics and performance indicators used to evaluate loan portfolios, customer behavior, and overall risk exposure. Mastery of these elements enables effective decision-making, strategic planning, and optimization of lending practices within the banking sector.

#### How do Banks Collect Loan Data?
Banks collect loan data through various channels, including loan applications, credit reports, income verification, collateral evaluation, and online platforms.

#### Process of Granting a Loan
The process of granting a loan typically involves the following steps: application, documentation, credit assessment, underwriting, approval, loan agreement, funding, loan servicing, risk management, and closure.

#### Reasons for Analyzing Bank Loan Data
Analyzing loan data is crucial for banks as it enhances several key areas of their operations. Firstly, it strengthens risk management by providing insights into potential default risks and loan performance, allowing banks to implement preventative measures and manage their risk exposure effectively. Secondly, it supports informed decision-making by offering data-driven insights into loan portfolios, enabling more strategic planning and targeted interventions. Performance monitoring is also significantly improved, as banks can track various metrics related to loan repayment and portfolio health, identifying trends and areas for improvement. Additionally, loan data analysis plays a critical role in fraud detection by uncovering anomalies and patterns indicative of fraudulent activity, thus safeguarding the institution’s assets. Finally, it provides valuable customer insights, helping banks understand borrower behavior and preferences, which can enhance customer relationship management and tailor financial products to meet customer needs more effectively.

### About Dataset
The dataset used in this analysis contains information about loan applicants, including attributes such as credit score, income, employment length, loan amount, and loan status.

#### Data Set Descriptions:
- **application_id**: A unique identifier for each loan application or borrower.
- **address_state**: The state where the borrower resides or where the loan originated.
- **application_type**: The type of loan application, which could be individual or joint (if multiple applicants are involved).
- **emply_length**: The length of employment for the borrower, typically measured in years.
- **emply_title**: The job title or occupation of the borrower.
- **loan_grade**: The risk grade assigned to the loan by the lending institution, usually based on the borrower's creditworthiness.
- **home_ownership**: The type of home ownership status of the borrower, such as own, mortgage, rent, etc.
- **issue_date**: The date when the loan was issued or originated.
- **last_credit_pull_date**: The date when the lender last pulled the borrower's credit report.
- **last_payment_date**: The date of the last payment made by the borrower.
- **loan_status**: The current status of the loan, such as fully paid, charged off, in default, etc.
- **next_payment_date**: The date of the next scheduled payment on the loan.
- **member_id**: A unique identifier for each member or borrower.
- **loan_purpose**: The purpose of the loan, such as debt consolidation, home improvement, medical expenses, etc.
- **sub_grade**: A more granular classification of the loan grade, typically used in credit scoring systems.
- **loan_term**: The duration of the loan, usually measured in months (e.g., 36 months, 60 months).
- **verification_status**: Whether the borrower's income and other information have been verified by the lender.
- **annual_income**: The annual income of the borrower.
- **dti**: The debt-to-income ratio, which measures the borrower's total monthly debt payments relative to their gross monthly income.
- **loan_installment**: The monthly payment amount due on the loan.
- **int_rate**: The interest rate charged on the loan.
- **loan_amount**: The total amount of the loan disbursed to the borrower.
- **total_acc**: The total number of credit accounts the borrower has.
- **total_payment**: The total amount paid by the borrower over the life of the loan.

Problem Statement

The objective of this project is to perform a comprehensive analysis of bank loan data using SQL and create key performance indicator (KPI) metrics to assess loan portfolio performance.

Dashboard 1: Summary
![BankLoanAnalysisSummary](https://github.com/user-attachments/assets/55b4c7f4-1d0b-4583-881c-11174178a6b2)

Key Performance Indicators (KPIs) Requirements:
- Total Loan Applications
- Total Funded Amount
- Total Amount Received
- Average Interest Rate
- Average Debt-to-Income Ratio (DTI)
  
Summary Dashboard

Dashboard 2: Overview
![BankLoanAnalysisOverview](https://github.com/user-attachments/assets/fa3a6698-b480-4775-a794-f0a5c8ffe367)

Charts
- Monthly Trends by Issue Date (Line Chart)
- Regional Analysis by State (Filled Map)
- Loan Term Analysis (Donut Chart)
- Employee Length Analysis (Bar Chart)
- Loan Purpose Breakdown (Bar Chart)
- Home Ownership Analysis (Tree Map)
  
**Overview Dashboard**

### Dashboard 3: Details
![BankLoanAnalysisDetails](https://github.com/user-attachments/assets/7a4f107a-7abf-4009-b57a-21b0c9504aae)

#### Grid
The Details Dashboard provides a consolidated view of key loan-related metrics and data points, enabling users to access critical information efficiently.

**Details Dashboard**

### Conclusion

The bank loan analysis offers a succinct yet insightful overview of loan portfolio performance, customer behavior, and risk assessment. Utilizing SQL for robust data processing and Power BI for dynamic visualization, this analysis provides actionable insights into trends in loan repayment, probabilities of default, and customer segmentation. By integrating data-driven decision-making into operational strategies, the bank can optimize lending practices, mitigate risks effectively, and enhance overall financial performance.

**MY APPRECIATION TO DATA TUTORIAL FOR PROVIDING THE DATASET AND GUIDIANCE IN DOING THIS PROJECT.
