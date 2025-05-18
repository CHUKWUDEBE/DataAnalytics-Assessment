DataAnalytics-Assessment

This repository contains my SQL solutions for a Data Analyst assessment designed to evaluate proficiency in querying and analyzing relational databases.

Repository Structure

Question-by-Question Explanation

Q1: High-Value Customers with Multiple Products
-  Approach: Used `JOIN` to match customers with both savings and investment plans. Filtered on funded accounts and aggregated deposits.
-  Challenge: Ensuring both account types are correctly linked using filters like is_regular_savings and  is_a_fund .

Q2: Transaction Frequency Analysis
-  Approach: Calculated monthly transactions per customer using a `WITH` clause, then grouped and categorized them based on average.
-  Challenge: Managing accurate monthly grouping and proper classification logic.

Q3: Account Inactivity Alert
- Approach: Used `LEFT JOIN` to compare transaction dates against today’s date and flag any accounts with no inflows in over a year.
- Challenge: Proper date calculations and identifying the correct transaction type fields.

Q4: Customer Lifetime Value (CLV)
- Approach: Combined account tenure and transaction data to estimate CLV using a simplified formula.
-Challenge: Proper division and avoidance of zero-division when tenure = 0.

Notes

All monetary values are converted from Kobo to Naira.
confirmed_amount was used for inflow references.
Only `SELECT` queries were used as per the instructions.
