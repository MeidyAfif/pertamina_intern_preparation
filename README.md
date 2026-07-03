# Training for Pertamina Intern Preparation: Fraud Detection EDA

**Author:** Meidy Afif Maulana  
**Target Role:** Data Analyst / Internal Audit Intern at Pertamina  
**Tech Stack:** Python, Pandas, NumPy, Matplotlib, Seaborn  

## Project Overview
This repository contains the Exploratory Data Analysis (EDA) phase of a financial fraud detection project. I worked on this specifically to prepare for the Pertamina Internship Program, focusing on finding anomalies and analyzing data from an internal audit perspective.

The dataset has over 6.3 million rows of financial transaction logs recorded over 31 days.

## Key Findings
1. **Structured Modus Operandi:** 100% of the 8,213 fraud cases only used TRANSFER and CASH_OUT methods to sever tracking trails.
2. **System Glitch Exploitation:** By calculating the balance logic, I found that fraudsters could cash out large amounts without the system reducing their original balance. 
3. **Legacy System Failure:** The existing alarm system (isFlaggedFraud) failed to detect most of these attacks, showing that a rule-based system is no longer enough.
4. **Active Hours:** Fraud activities peak between 02:00 AM and 04:00 AM, proving that these attacks target vulnerable monitoring hours or use automated scripts.

## Next Steps
* Data Preprocessing and Feature Encoding.
* Handling Imbalanced Data using SMOTE.
* Building a Machine Learning classification model to automate fraud detection.
