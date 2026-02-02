# Data-cleaning-on-MS-Excel
A dirty cafe dataset with missing values and poorly formatted values was cleaned on Microsoft Excel using simple formulas. The aim of this data cleaning project was not to fill every empty space but to clean the data while maintaining data intergrity.

INTRODUCTION: The aim of this project was to clean a dirty cafe dataset, replace missing values where possible, remove rows with numerous null values and fill null rows where possible. The dataset was synthetically produced to provide realistic scenario for data cleaning and Exploratory Data Analysis (EDA).

This dataset was downloaded from Kaggle. It contains 10, 000 rows of synthetic data representing sales transaction in a cafe. The rows included in this data are: Transaction ID, Items, Quantity, Price per Unit, Total Spent Payment Method, Location and Transaction Date, each of which contained missing rows.
This missing rows could have been handled using Power Query, however, using Power Query without a keen eye would affect data integrity which must be maintained to ensure data analysis and visualization. Using IFERROR formula I was able to fix calculation failures in the numeric columns. In order to avoid DIV/0! and VALUE! errors while using this formula, I changed the BLANK, UNKNOWN and ERRORS to actual blank rows, that way using IFERROR eliminates errors.

The formula usage : IFERROR formula was used to fic calculation fixtures in PRICE PER UNIT, QUANTITY AND TOTAL SPENT columns. 
IF function was used to fill in blank spaces in the ITEMS column using the Price Per Unit column as a reference.

DIRTY CAFE COPY
<img width="1363" height="698" alt="Screenshot 2026-01-22 115840" src="https://github.com/user-attachments/assets/7538f836-55c5-4689-8fb6-8125dd6828b6" />

CLEANED CAFE COPY
<img width="1366" height="698" alt="Screenshot 2026-01-22 120157" src="https://github.com/user-attachments/assets/32c0822f-2915-4a72-b519-f68f4a3812c9" />

At the end of this data cleaning project, all the fillable rows were filled. In order to avoid conflict and to preserve data integrity, not all rows were forcibly filled.



