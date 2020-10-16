# HireArt-Data_Analysis_Assessment

Problem Statement:
The marketing ops team sent over this spreadsheet containing four years of data from a CRM system (please make a copy of the spreadsheet in order to manipulate the data): https://docs.google.com/spreadsheets/d/16hLtx8bBDe2GS1MOa3v9hY6Yhm4C30koLoCpiIJ5WDg/edit?usp=sharing.

The team wants to find the month they're likely to contact the most clients, so they can schedule a product upgrade announcement. Which month does the team tend to contact the greatest percentage of its clients?

Solution Approach:
1) Firstly, gathered the data by opening the spreadsheet url given on a local machine, and saw the data. Then downloaded the data in form of .csv file, and saved a copy of it on my local machine.

2) Then, read the .csv file with read_csv into dataframe using Jupyter Notebook and displayed first 5 rows of it.

3) Now performed preliminary wrangling on the data to check and assess quality and tidiness issues. 

4) After assessing the data, I found that the 'Date of Contact' column need to be converted to datetime format for better analysis of the data. 

Assessment of Data
> We found that the data consists of 3 columns with 1001 row entries.
> The data type of 'Date of Contact' column should be datetime instead of object.
> There are 35 unique clients, 4 unique account managers and 704 unique dates in this data set.
> Also it seems that **October** month might have maximum number of client contacted, but lets explore it more to confirm the analysis.

5) So, I changed the data type to datetime format and also melted the 'Date of contact' column to date, month and year as we need to find the suitable month for product upgrade announcement.

6) Finally, I perfomed exploratory Data Analysis by grouping the clients with month to find the maximum number of clients contacted per month. Also, analysed the maximum number of unique clients contacted in which month. 

7) After successful analysis, I also performed Data Visualization to get better insights about the analysis.

After Data Analysis, I can conclude that in October month all 35 unique clients are contacted. Also it can be inferred from the analysis that to contact maximum number of clients, October is the best suitable month with 100% clients. 

Hence, as per the conclusion drawn from above, team should schedule the product upgrade announcement in October month to reach out to maximum number of clients successfully.
