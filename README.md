# Crowdfunding-ETL

## Overview of project

- The purpose of the project is to perform an ETL process on a new dataset that contains information about the backers who’ve pledged to the live projects and perform data analysis by using SQL queries.


## Sources

- Data:

	1. [crowdfunding]()
	2. [backers_info]()
	
- Softwares: Anaconda 22.9.0, Python 3.7.6 Jupyter Notebook 6.4.12, QuickDBD and Postgressql 14.6

## Analysis

- The script for phase 1 & 2 analysis is: [Extract-Transform_final_code]() 

### Phase 1

- In this phase, the data is extracted from the file and converted into a readable format

- The link to the dat file with option 1 is [backers_data1]()

- The link to the dat file with option 2 is [backer_data2]()

- The extracted data is 

![backer_data]()

### Phase 2

- In this phase, the data from phase 1 is transformed to make it more structured for analysis. The link to the data file is [backers]()

- The transformed data is 

![final_backers]()

### Phase 3

- The ERD model used to include the above table is shown below

![crowdfunding_db_relationships]()

 - The link to the ERD file is [ERD_code]()

- In this phase, an SQL query is written in Postgres to create a new table and import the data from the above file. The link to the queries is [crowdfunding_db_table_schema]()

- The created table is shown below

![backers]()


### Phase 4

- The link to the queries is [crowdfunding_SQL_Analysis]()

- Analysis is performed to find all contacts of each live campaign and calculate the "remaining goal amount". 

- The created table is shown below

![email_contacts_remaining_goal_amount]()

- Analysis is performed to find all backers for each live campaign and calculate the remaining goal amount as "Left of goal".

- The created table is shown below

![email_backers_remaining_goal_amount]()
