# Telecom Customer Churn Analysis

## Project Overview

This project uses Python to clean and analyze customer-level telecommunications data to investigate patterns associated with customer churn.

The analysis examines customer status, contract structure, tenure, monthly charges, internet services, security services, and reported reasons for leaving.

The goal was to demonstrate a structured Python workflow covering data preparation, exploratory data analysis, visualization, and communication of business findings.

---

## Tools & Skills

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Data Cleaning
- Exploratory Data Analysis
- Data Validation
- Data Visualization
- Customer Churn Analysis
- Business Analysis

---

## Business Objective

The analysis was designed to investigate questions such as:

- What percentage of customers have churned?
- How does churn vary by contract type?
- How does customer tenure relate to churn?
- How do monthly charges differ between churned and retained customers?
- How does churn differ based on internet service?
- How does churn vary with adoption of services such as Online Security?
- What reasons do customers report for leaving?
- Which categories account for the largest share of reported churn?

---

## Data Preparation

Before performing the analysis, the dataset was reviewed for missing values, structural inconsistencies, and potential anomalies.

Several missing values represented fields that were not applicable to particular customers rather than unknown information.

Examples included:

- Churn reason fields for customers who had not churned
- Internet-related fields for customers without internet service
- Phone-related fields for customers without phone service

Where appropriate, categorical fields were classified as **Not Applicable**, while selected numeric usage fields were assigned values consistent with the absence of the corresponding service.

<img width="1734" height="1476" alt="image" src="https://github.com/user-attachments/assets/9bc071f9-6a90-427a-9b91-254f30d05349" />


Potential anomalies in monthly charges were also reviewed. Because the negative values affected a small subset of customers and were limited in magnitude, they were retained rather than modified without evidence that they represented data-entry errors.

---

## Exploratory Analysis

### Overall Churn

Approximately **26.5%** of customers in the dataset had churned.

<img width="1708" height="1480" alt="image" src="https://github.com/user-attachments/assets/0b53eb2d-3c36-41f8-9586-2b39e85fcf86" />
<img width="1720" height="1522" alt="image" src="https://github.com/user-attachments/assets/7da8ef05-4d8e-4cda-95a6-b9f64bb02bb0" />
<img width="1608" height="1534" alt="image" src="https://github.com/user-attachments/assets/a1de9b04-ecc4-4959-8384-2d7128a9ab8b" />
<img width="1394" height="1530" alt="image" src="https://github.com/user-attachments/assets/73f26692-d7ed-4ec9-9a68-24015b4e335d" />
<img width="1500" height="1236" alt="image" src="https://github.com/user-attachments/assets/1bce92f0-c4c7-4e42-a4be-31f547d55755" />
<img width="1716" height="1504" alt="image" src="https://github.com/user-attachments/assets/60ceb50c-9fe2-4bc0-8af2-f36351258c96" />
<img width="1726" height="1520" alt="image" src="https://github.com/user-attachments/assets/cc92a0f1-559e-4b31-b571-00eca237a667" />
<img width="1718" height="1216" alt="image" src="https://github.com/user-attachments/assets/f6668fae-5a33-44f2-a057-a33f3fb8b5ae" />


### Contract Type

Churn varied substantially by contract structure:

- Month-to-month: approximately 45.8%
- One-year: approximately 10.7%
- Two-year: approximately 2.6%

<img width="1722" height="1330" alt="image" src="https://github.com/user-attachments/assets/c412e400-be16-4d3e-a8a8-02bb86237d47" />


Customers with month-to-month contracts therefore exhibited a substantially higher churn rate within the dataset than customers with longer-term contracts.

---

## Tenure

Churn rates were analyzed across customer tenure to investigate how customer longevity relates to retention.

<img width="1724" height="1244" alt="image" src="https://github.com/user-attachments/assets/40589c45-6f8f-46e9-abe1-083c3db29cc0" />


The analysis identified meaningful differences in churn across tenure groups, providing additional context around when customer attrition is most prevalent.

---

## Monthly Charges

Churned customers had higher average monthly charges than customers who remained:

- Churned customers: approximately $73
- Retained customers: approximately $62

<img width="1712" height="344" alt="image" src="https://github.com/user-attachments/assets/c6629088-522f-4fa0-a414-30aaabda5697" />


This represents an association within the dataset and does not by itself establish that higher monthly charges cause churn.

---

## Services

Churn also varied based on service adoption.

Customers with internet service had a churn rate of approximately **31.8%**, compared with approximately **7.4%** among customers without internet service.

Online Security showed another substantial difference:

- Without Online Security: approximately 41.8% churn
- With Online Security: approximately 14.6% churn

These differences identify customer segments that may warrant further investigation.

---

## Churn Categories & Reasons

Reported churn reasons were analyzed to better understand why customers indicated they had left the company.

<img width="1712" height="1214" alt="image" src="https://github.com/user-attachments/assets/81f12872-9940-4487-863d-cf0a0f2342ec" />


Competitor-related factors represented approximately **45%** of reported churn.

The two most frequently reported individual reasons were:

1. Competitor had better devices
2. Competitor made a better offer

<img width="1726" height="1392" alt="image" src="https://github.com/user-attachments/assets/7343ec9a-444c-4d42-a068-8195df97a2aa" />


---

## Key Business Findings

The analysis identified several notable patterns:

- Approximately one-quarter of customers had churned.
- Month-to-month customers had substantially higher churn than customers with longer-term contracts.
- Churned customers had higher average monthly charges than retained customers.
- Churn rates differed considerably based on internet service and Online Security adoption.
- Competitor-related factors represented the largest category of reported churn.
- Better competitor devices and offers were the two most frequently reported individual reasons for leaving.

These findings identify areas that could be investigated further with additional business context and customer information.

---

## Project Outcome

The completed analysis demonstrates a structured Python workflow for cleaning customer-level data, validating missing values and anomalies, conducting exploratory analysis, creating visualizations, and communicating findings in a business context.

The analysis focuses on identifying patterns present in the data without treating observed relationships as evidence of causation.

---

## Data Source

This project uses the Telecom Customer Churn dataset provided by Maven Analytics.

The dataset was used for portfolio and educational purposes.

---

## Jupyter Notebook

The complete Python analysis is available in this project folder:

`customer_churn_analysis.ipynb`
