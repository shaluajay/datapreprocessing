Marketing Campaign Data Cleaning Report

This document summarizes the steps taken to clean and prepare the Marketing Campaign dataset (marketing_campaign.csv) for analysis. The cleaning process focused on handling missing values, standardizing entries, fixing data types, and creating new, useful features.

Cleaning and Preparation Steps
1. Handling Missing Values
Income: Missing values were imputed using the median income value.

Dt_Customer: Standardized and converted to proper datetime format.

2. Removing Duplicates
Duplicate rows were identified and removed to ensure data integrity.

3. Standardizing Text Values
Education:

"2n Cycle" standardized to "Master".

"Basic" standardized to "Undergraduate".

Marital_Status:

"Alone" standardized to "Single".

"Together" standardized to "Married".

4. Converting Date Formats
Dt_Customer was parsed into a proper datetime object using the format %d-%m-%Y.

5. Renaming Column Headers
All column headers were converted to lowercase and underscores for consistency and readability.

6. Fixing Data Types
year_birth: Converted to integer.

income: Filled missing values and converted to float.

Dt_Customer: Converted to datetime.

7. Feature Engineering
New columns were created:

age: Current year minus year_birth.

total_children: Sum of kidhome and teenhome.

total_spending: Total spending across various product categories.

total_purchases: Total purchases across different channels.

Final Verification:

1)Ensured correct data types for all columns.

2)Confirmed no missing values remained.

3)Inspected sample records to verify changes.

