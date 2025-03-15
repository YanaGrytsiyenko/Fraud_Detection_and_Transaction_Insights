# Fraud Detection & Transaction Insights

## Project Description

This project is aimed at analyzing fraudulent transactions and gaining insights into transactions and the system that detects them. Using Python and Tableau, I processed data for analysis and visualization, which allows identifying key aspects and anomalies.

The project contains two Jupyter notebooks:
- **`UKR_Fraud_Detection_&_Transaction_Insights.ipynb`**: The Ukrainian version of the project that includes the entire process of analyzing fraudulent transactions.
- **`ENG_Fraud_Detection_&_Transaction_Insights.ipynb`**: The English version of the project for an international audience with the same analysis process.

The project also includes an interactive **[Tableau dashboard](https://public.tableau.com/views/Project_17417206273100/FraudDetectionTransactionInsights?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**, available on the Tableau Public platform, where you can visualize key metrics and analysis results.

## Table of Contents
1. [Data Overview](#data-overview)
2. [Tools and Technologies](#tools-and-technologies)
3. [Data Analysis Workflow](#data-analysis-workflow)
4. [Key Findings](#key-findings)
5. [Contacts](#contacts)

## Data Overview

**Source**: [Dataset](https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset/data)  
**Size**: 6,362,620 rows and 11 columns.

### Key Fields:
- **`step`**: a unit of time, where 1 step equals 1 hour.
- **`type`**: the type of online transaction.
- **`amount`**: the transaction amount.
- **`nameOrig`**: the client who initiates the transaction.
- **`oldbalanceOrg`**: balance before the transaction.
- **`newbalanceOrig`**: balance after the transaction.
- **`nameDest`**: the recipient of the transaction.
- **`oldbalanceDest`**: the initial balance of the recipient before the transaction.
- **`newbalanceDest`**: the new balance of the recipient after the transaction.
- **`isFraud`**: fraudulent transaction.
- **`isFlaggedFraud`**: system flag marking this as a fraudulent transaction.

**Last data update**: 2022.  
**Data downloaded**: The data was downloaded from [Google Drive](https://drive.google.com/file/d/1AhnMI7DsFwXGb3aisYj1p7DVExXEB_0x/view?usp=sharing). 

## Tools and Technologies

- **Python**: For additional data transformations and visualizations.
  - Data manipulation: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  
- **Tableau**: For creating visualizations and dashboards.

- **Google Colab**: For writing and executing Python scripts.

- **GitHub**: Repository for the project code and documentation.

## Data Analysis Workflow

1. **Data Cleaning**: 
   - Removal of missing values.
   - Conversion of categorical variables to numerical.

2. **Analysis**: 
   - Formulating questions for analysis and searching for answers.

3. **Visualization**: 
   - Creating plots using Python.
   - Building an interactive Tableau dashboard.

## Key Findings

📌 The system likely has a limited threshold for marking suspicious transactions (around 5 million UAH), so fraudsters may split large amounts into smaller payments to avoid detection.

📌 The system detects only 0.19% of fraudulent transactions, indicating a need for model improvement.

📌 More attention is needed for **CASH_OUT** and **TRANSFER** transactions, as they are the most commonly used by fraudsters.

📌 It is important to monitor clients who were previously detected as fraudsters, as they might perform further transactions that the system no longer detects.

📌 It is recommended to add new columns to the data, such as:
   - Transaction dates.
   - Countries or regions.
   - Bank information.
   - Transaction duration and other relevant data.

## Contacts

For any questions or feedback, feel free to contact me:
- **Name**: Yana Grytsiyenko
- **Email**: [yanakoziuchenko@gmail.com](mailto:yanakoziuchenko@gmail.com)
- **GitHub**: [github.com/YanaGrytsiyenko](https://github.com/YanaGrytsiyenko)
- **LinkedIn**: [linkedin.com/in/yanakoziuchenko/](https://www.linkedin.com/in/yanakoziuchenko/)
