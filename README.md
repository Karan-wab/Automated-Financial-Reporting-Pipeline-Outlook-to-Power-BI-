# Automated-Financial-Reporting-Pipeline-Outlook-to-Power-BI-

# Automated Financial Reporting and Analytics Dashboard

## 1. Project Goal
The goal of this project is to automate a manual daily reporting process and build an interactive Power BI dashboard. This solution aims to save time, reduce operational costs, eliminate human error, and provide deep financial insights to management.

---

## 2. Problem Statement
The existing workflow involved manually downloading 25 files from email every day, combining them, and cleaning the data before a dashboard could be built. This process faced several critical challenges:
* **Time-Consuming**: The manual data preparation took hours, risking delays in the final report.
* **High Costs**: An additional $12,000 per month was spent on staff to manage this workload.
* **High Error Rate**: Manual data manipulation led to frequent errors, compromising data accuracy.
* **Inefficiency**: The heavy workload on this single task was negatively impacting other company projects.

---

## 3. The Solution
An automated, two-part solution was developed:

### A. Python Data Pipeline
A Python script automates the entire data collection and preparation phase.
* It securely connects to a specific Google Drive folder using the Google Drive API.
* It identifies and downloads all the required daily financial files, handling different formats (CSV, Excel, Google Sheets).
* Using the Pandas library, it combines and cleans the data, preparing a master dataset for analysis.

### B. Power BI Dashboard
The cleaned data is visualized in an interactive Power BI dashboard that provides answers to key business questions, including:
* Calculation of customer **Lifetime Value (LTV)** scores.
* Analysis of loan and credit card ownership across different age groups.
* Identification of the most popular loan products.
* Insights into customer inquiry patterns and payment delays.

---

## 4. Tech Stack & Tools
* **Data Automation**: Python, Pandas, Google Drive API
* **Dashboarding & BI**: Microsoft Power BI

---

## 5. File Descriptions
* `Financial Dashboard.docx`: The project requirements document, outlining the business problem and the analytical questions to be answered.
* `Financial_Notepad.docx`: Contains the Python script used for automating the data pipeline from Google Drive.
* `financial-project-drive-bridge-87e32fc7d02b.json`: The service account credentials for the Google Drive API (for authentication).
* `Financial Project.pbix`: The final, interactive Power BI dashboard file.

---

## 6. How to Use

### A. Data Pipeline
1.  Ensure you have Python and the necessary libraries installed (`pandas`, `google-api-python-client`, etc.).
2.  Set up a Google Cloud Platform project with the Drive API enabled.
3.  Place the `financial-project-drive-bridge-87e32fc7d02b.json` credentials file in the same directory as the script.
4.  Run the Python script from `Financial_Notepad.docx` to fetch and process the data.

### B. Viewing the Dashboard
1.  You must have **Microsoft Power BI Desktop** installed.
2.  Open the `Financial Project.pbix` file.
3.  The dashboard will load with all the data and visuals, ready for interactive analysis.

---

## 7. Dashboard Features & KPIs
The dashboard is designed to provide strategic insights at a glance:
* **LTV Score Analysis**: Visuals showing LTV scores for different age groups, with conditional formatting to highlight customer tiers for targeted promotions.
* **Loan Product Analysis**: Charts displaying the popularity of different loan types.
* **Credit Usage by Age**: Analysis of the average number of loans and credit cards held by customers across various age brackets.
* **Customer Behavior Metrics**: KPIs on average payment delays, credit scores, and investment amounts to provide a holistic view of the customer base.
