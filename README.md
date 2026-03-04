🏠 Airbnb Data Cleaning Pipeline
📌 Project Overview

This project builds a professional end-to-end data cleaning pipeline for the Airbnb Open Data dataset. The objective is to transform raw, messy data into a clean, reliable, and analysis-ready dataset suitable for exploratory data analysis (EDA) and machine learning workflows.

The pipeline follows industry best practices in data preprocessing, validation, and feature preparation.

🎯 Objectives

Improve data quality and consistency

Remove irrelevant and redundant features

Handle missing and duplicate records

Standardize categorical and numerical variables

Prepare the dataset for downstream analytics and modeling

🗂️ Dataset

Source: Airbnb Open Data
Format: CSV
Main focus: Listings, host information, pricing, and reviews

🔧 Data Cleaning Steps
1️⃣ Column Selection

Removed low-value and irrelevant columns

Kept only features useful for analysis

2️⃣ Column Standardization

Converted column names to uppercase

Trimmed whitespace for consistency

3️⃣ Duplicate Removal

Removed full duplicate rows

Prevented data inflation and bias

4️⃣ Missing Value Handling

Applied targeted NaN removal on critical fields (LAST REVIEW, NAME)

⚠️ Note: Removing all NaNs globally would reduce the dataset to a single row

5️⃣ Feature Cleaning & Encoding

HOST_IDENTITY_VERIFIED → binary encoding (1/0)

INSTANT_BOOKABLE → binary encoding (1/0)

CANCELLATION_POLICY → ordinal encoding

flexible = 1

moderate = 2

strict = 3

Cleaned monetary fields:

Removed $ and ,

Converted to numeric

6️⃣ Data Quality Checks

Reviewed data types

Checked remaining missing values

Generated statistical summary

Inspected numeric ranges for anomalies

🧪 Technologies Used

Python 🐍

Pandas

Jupyter Notebook

📊 Final Outcome

The dataset is now:

✅ Clean
✅ Consistent
✅ Properly encoded
✅ Analysis-ready

It can be directly used for:

Exploratory Data Analysis (EDA)

Dashboarding (Power BI / Tableau)

Feature engineering

Machine learning models

🚀 How to Run
# Clone the repository
git clone <your-repo-url>

# Install dependencies
pip install pandas

# Run the notebook or script
📌 Future Improvements

Outlier detection and treatment

Feature engineering

Automated data validation tests

Data pipeline modularization

Integration with BI dashboards

👩‍💻 Author

Adriana Celeste
Data Scientist | BI Developer | Python
