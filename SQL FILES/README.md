Hospital Encounter Data Analysis (SQL Project)
Overview
This project analyzes patient encounters from a hospital database to uncover trends in patient admissions,
encounter types, cost distribution, and readmission behavior.
 It demonstrates practical use of SQL for healthcare data analytics — from performance metrics to patient behavior insights.

Dataset Description
Table: encounters
 Fields:
PATIENT: Unique ID of each patient


START / STOP: Encounter start and end times


ENCOUNTERCLASS: Type of encounter (e.g., ambulatory, inpatient, emergency)


BASE_ENCOUNTER_COST / TOTAL_CLAIM_COST: Financial data for each encounter


PAYER / PAYER_COVERAGE: Insurance information


CODE / REASONCODE: Procedure and reason codes



Key Business Questions & Analysis
How many total encounters occurred each year?


What percentage of encounters belonged to each encounter class (ambulatory, inpatient, etc.)?


What percentage of encounters lasted over 24 hours vs under 24 hours?


How many encounters had zero payer coverage?


What are the top 10 most frequent and most expensive procedures?


What is the average total claim cost per payer?


How many unique patients were admitted each quarter?


How many patients were readmitted within 30 days?


Which patients had the most readmissions?



SQL Techniques Used
Aggregation & Filtering: COUNT(), AVG(), SUM(), ROUND(), WHERE


Time-based Analysis: YEAR(), MONTH(), QUARTER(), DATEDIFF()


Window Functions: OVER (PARTITION BY ...) for percentage analysis


Joins: Used for readmission and patient behavior tracking


Case Statements: Categorizing encounter durations (>24 hours / ≤24 hours)


Ranking & Limiting: ORDER BY ... LIMIT 10 for top procedures and patients



Key Insights
 Encounter Trends: Encounters increased steadily across years, showing hospital growth.


 Encounter Classes: Outpatient and ambulatory visits make up the majority of encounters, indicating focus on non-emergency services.


 Duration Insight: About 70–80% of encounters lasted less than 24 hours, meaning most treatments are short-term.


 Zero Payer Coverage: A small but significant percentage of encounters (typically 3–5%) had no insurance coverage.


 Frequent Procedures: Common low-cost procedures dominate, while specialized ones are fewer but more expensive.


 Top Payers: Certain payers show higher average claim costs, reflecting cost variations in insurance plans.


 Patient Behavior: A small subset of patients had multiple readmissions within 30 days, suggesting the need for improved follow-up care.



Skills Demonstrated
SQL Data Analysis | Healthcare Data Analytics | Aggregation & Joins | Window Functions | Business Insight Reporting

Recommendation
Enhance post-discharge follow-up programs to reduce frequent readmissions.


Expand outpatient and wellness services, as they form the largest encounter category.


Investigate high-cost procedures and negotiate better payer coverage terms.


Target uninsured patients with financial assistance programs to improve coverage rates.

