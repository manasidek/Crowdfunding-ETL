# Crowdfunding-ETL

## Overview of project

- The purpose of the project is to perform an ETL process on a new dataset that contains information about the backers who’ve pledged to the live projects and perform data analysis by using SQL queries.


## Sources

- Data:

	1. [crowdfunding](https://github.com/manasidek/Crowdfunding-ETL/blob/main/DATA/crowdfunding.xlsx)
	2. [backers_info](https://github.com/manasidek/Crowdfunding-ETL/blob/main/DATA/backer_info.csv)
	
- Softwares: Anaconda 22.9.0, Python 3.7.6 Jupyter Notebook 6.4.12, QuickDBD and Postgressql 14.6

## Analysis

- The script for phase 1 & 2 analysis is: [Extract-Transform_final_code](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Code_and_Queries/Extract-Transform_final_code.ipynb) 

### Phase 1

- In this phase, the data is extracted from the file and converted into a readable format

- The link to the data file with option 1 is [backers_data1](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Data/backers_data1.csv)

- The link to the data file with option 2 is [backers_data2](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Data/backers_data2.csv)

- The extracted data is:

![backer_data](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/backer_data.png)

### Phase 2

- In this phase, the data from phase 1 is transformed to make it more structured for analysis. The link to the data file is [backers](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Data/backers.csv)

- The transformed data is 

![final_backers](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/final_backers.png)

### Phase 3

- The ERD model used to include the above table is shown below

![crowdfunding_db_relationships](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/crowdfunding_db_relationships.png)

 - The link to the ERD file is [ERD_code](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Code_and_Queries/ERD_code.txt)

- In this phase, an SQL query is written in Postgres to create a new table and import the data from the above file. The link to the queries is [crowdfunding_db_table_schema](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Code_and_Queries/crowdfunding_db_table_schema.sql)

- The created table is shown below

![backers](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/backers.png)


### Phase 4

- The link to the queries is [crowdfunding_SQL_Analysis](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Code_and_Queries/crowdfunding_SQL_Analysis.sql)

- Analysis is performed to find all contacts of each live campaign and calculate the "remaining goal amount". The link to the csv is: [email_contacts_remaining_goal_amount](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Data/email_contacts_remaining_goal_amount.csv)

- The created table is shown below

![email_contacts_remaining_goal_amount](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/email_contacts_remaining_goal_amount.png)

- Analysis is performed to find all backers for each live campaign and calculate the remaining goal amount as "Left of goal". The link to the csv is: [email_backers_remaining_goal_amount](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Data/email_contacts_remaining_goal_amount.csv)

- The created table is shown below

![email_backers_remaining_goal_amount](https://github.com/manasidek/Crowdfunding-ETL/blob/main/Images/email_backers_remaining_goal_amount.png)
