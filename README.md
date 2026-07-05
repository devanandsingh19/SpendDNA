# 💳 SpendDNA - Personal Finance Transaction Analysis

SpendDNA is a Python-based data analytics project that transforms raw bank transaction data into meaningful financial insights. Using a synthetic dataset of a Bengaluru software engineer, the project cleans transaction records, identifies vendors, categorizes expenses, analyzes spending behavior, detects anomalies, and generates a comprehensive financial report.

This project was completed as part of the **Unlox Academy SpendDNA Minor Project**.

---

## 📌 Project Overview

The objective of this project is to analyze six months of banking transactions and answer questions such as:

- Where is most of the money being spent?
- Which merchants are used the most?
- How healthy are the user's spending habits?
- Are there any unusual transactions?
- What kind of spender is the user?

The final output is a console-based financial report summarizing the user's spending behavior.

---

## 📂 Dataset

**File:** `rahul_transactions.csv`

The dataset contains synthetic bank transactions of a fictional Bengaluru software engineer.

**Dataset Information**

- Duration: January 2024 – June 2024
- Total Transactions: 1,310 (after removing duplicates)
- Multiple date formats
- Mixed amount formats
- UPI, Card, ATM and Net Banking transactions
- Realistic merchant descriptions

---

## 🚀 Features

### 1. Data Cleaning & Preprocessing
- Removed duplicate transactions
- Converted multiple date formats into datetime
- Cleaned currency values
- Standardized transaction types
- Created time-based features

### 2. Vendor Identification
Extracted canonical vendors from noisy transaction descriptions using keyword mapping.

Example:

```
SWIGGY-INSTAMART
↓
Swiggy Instamart

UPI-AMZN
↓
Amazon
```

---

### 3. Transaction Categorization

Mapped vendors into categories such as:

- Food Delivery
- Quick Commerce
- Groceries
- Ecommerce
- Restaurants
- Cafe
- Transport
- Fuel
- Investments
- Utilities
- Entertainment
- Rent
- Subscriptions
- Personal Transfer
- Cash Withdrawal

---

### 4. Spending Overview

Calculated:

- Total Credits
- Total Debits
- Net Savings
- Savings Rate
- Highest Spending Categories
- Top Vendors

---

### 5. Monthly Spending Trends

Analyzed monthly spending patterns for:

- Food Delivery
- Quick Commerce
- Ecommerce
- Investments

---

### 6. Time-of-Day Analysis

Identified spending behavior based on transaction time.

Examples include:

- Food Delivery after 9 PM
- Morning Cafe Visits
- Quick Commerce activity

---

### 7. Anomaly Detection

Detected unusually large transactions using **Z-Score**.

For each category:

- Mean
- Standard Deviation
- Z-score
- Top anomalous transactions

---

### 8. Spending Archetype Detection

Automatically classified the user into financial archetypes such as:

- 🍔 The Foodie
- 🛒 The Quick Commerce Junkie
- 🛍️ The Shopaholic
- 📈 The Investor
- 🌙 The Late-Night Snacker
- 🚕 The Cab Commuter
- 📺 The Subscription Lover
- 💸 The YOLO Spender
- 💰 The Disciplined Saver

---

### 9. SpendDNA Report

Generated a complete text-based financial report including:

- Executive Summary
- Spending Overview
- Top Categories
- Top Vendors
- Time-of-Day Patterns
- Monthly Trends
- Anomaly Detection
- Spending Archetypes
- Key Insights

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Datetime
- Jupyter Notebook

---

## 📊 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Wrangling
- Feature Engineering
- String Processing
- GroupBy Operations
- Financial Data Analysis
- Statistical Analysis
- Rule-Based Classification
- Report Generation

---

## 📁 Project Structure

```
SpendDNA/
│
├── rahul_transactions.csv
├── SpendDNA_Project.ipynb
├── SpendDNA_Report.txt
├── README.md
└── images/
```

---

## 📷 Sample Output

```
========================================================
SpendDNA REPORT - RAHUL SHARMA
========================================================

EXECUTIVE SUMMARY

Total Credits : ₹509,774
Total Debits  : ₹1,678,901
Savings Rate  : -229.3%

TOP CATEGORIES
• Ecommerce
• Investments
• Restaurants

TOP VENDORS
• Amazon
• Zerodha
• Flipkart

SPENDING ARCHETYPES
✔ THE SHOPAHOLIC
✔ THE YOLO SPENDER
```

---

## 🎯 Learning Outcomes

This project strengthened my understanding of:

- Real-world transaction data preprocessing
- Merchant normalization
- Category mapping
- Spending behavior analysis
- Statistical anomaly detection
- Rule-based analytics
- Building end-to-end data analytics projects using Python

---

## 👨‍💻 Author

**Dev Anand Singh**

Computer Science Engineering Student

---

## ⭐ If you found this project useful, consider giving it a star!
