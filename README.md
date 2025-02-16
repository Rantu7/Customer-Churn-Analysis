# Customer Churn Analysis – A Data-Driven Approach to Retention
Churn Analysis of a bank's customer dataset by Rantu Adhikary

Customer churn refers to the percentage of customers who stop using a company’s services over a given period. In the banking sector, churn happens when customers close their accounts, stop using financial products, or switch to a competitor. A high churn rate can negatively impact revenue, operational efficiency, and brand loyalty.

# Project Objective
This analysis aims to identify key factors influencing customer churn and provide actionable insights to improve customer retention. Using Power BI, this project visualizes customer behavior based on demographics, account balances, credit scores, and product usage.
By understanding these patterns, businesses can implement targeted strategies to enhance customer engagement, optimize product offerings, and ultimately reduce churn. This project will highlight the key findings and recommendations to support data-driven decision-making.

# About The Dataset:
The dataset contains a .csv file consisting of 14 columns related to customer activities and status. The columns are: Customer ID, Credit Score, Country, Gender, Age, Tenure, Balance, Products, Activity status, Churn Status, Age groups, Credit Score, Account Balance.

# The Dashboard:

It is a 2 page interactive dashboard where the first page focuses on showcasing the KPIs and an overview of the business with a churn status slicer, while the 2nd page presents the relationship among different variables.  Screenshots are given below: 

![Image](https://github.com/user-attachments/assets/4e8a6f91-0ede-4950-9bf8-76374c112174)
![Image](https://github.com/user-attachments/assets/6cd8cabe-91ce-4bcd-a494-d17ef7d90f02)

Downloadable power bi file link: https://github.com/Rantu7/Customer-Churn-Analysis/blob/main/Customer%20Churn%20bank.pbix

# DAX Formulas: 

Some simple Data Analysis Experssion (DAX) formulas were used to perform the necessary calculations. They are given below:

   ```dax
Churn Rate = [Customers Lost]/[Total Customers]
   ```

   ```dax
Customers Lost = CALCULATE(COUNT('Bank Customer Churn Prediction'[Churn Status]),'Bank Customer Churn Prediction'[Churn Status]="Churned")
  ```

   ```dax
Total Customers = COUNT('Bank Customer Churn Prediction'[Customer ID])
  ```

# Insights:

•	Churn Rate is 20.4%, which is beyond the acceptable threshold of 15%. This means a significant portion of customers are leaving. The company should investigate key drivers of churn and implement retention strategies.

•	Germany has the highest churn rate (32.4%), followed by Spain (16.7%) and France (16.2%). German customers are churning at a much higher rate. The company should assess local policies, competition, and customer satisfaction in Germany.

•	Customers with low balances (0-10K) have the highest churn rate (100%), while those with 100K-200K have a 55.9% churn rate. Customers with lower balances may feel disengaged or find better financial options elsewhere. Offering incentives, better services, or exclusive benefits for lower-balance customers could help retain them.

•	The highest churn occurs in customers with credit scores between 601 - 700. Customers in this credit score range may be struggling with financial stability. The company could introduce tailored financial assistance or loyalty programs.

•	The highest churn is among customers aged 41-50. This age group may require more personalized financial planning, family-oriented banking services, or better digital banking experiences.

•	Inactive customers (48.49%) are nearly equal to active ones (51.51%). A large portion of customers are inactive, meaning they might be at higher risk of churning. Proactive engagement strategies such as personalized offers, reminders, and value-driven interactions could help activate them.

•	Customers without credit cards (29.45%) might have a different risk profile. Encouraging more customers to use credit cards (with benefits) might increase engagement and reduce churn.

•	Customers with Product 4 (45.87%) and Product 3 (37.94%) have the highest churn rates.These products might not be delivering value, or customers might be switching to better alternatives. A product review and potential improvements are necessary.

# Recommendations

1.	Focus on Retaining German Customers: Investigate local factors driving churn.
2.	Target Low-Balance Customers: Provide incentives or better benefits to encourage loyalty.
3.	Improve Engagement for Middle-Age Customers (41-50): Offer personalized services to reduce churn.
4.	Re-engage Inactive Customers: Use targeted communication and loyalty programs.
5.	Enhance Product Offerings: Evaluate high-churn products and improve their value proposition.

## Thank You!

