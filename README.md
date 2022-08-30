Description of the project

Credit Card Dataset Overview - PART 1

This Capstone Project utlizes the following technologies to manage an ETL process for a Loan Application dataset and a Credit Card dataset: Python (Pandas, advanced modules e.g., Matplotlib), MariaDB, Apache Spark (Spark Core, Spark SQL), and Python Visualization and Analytics libraries.

Credit Card Dataset Overview The Credit Card System database is an independent system developed for managing activities such as registering new customers and approving or canceling requests, etc., using the architecture. A credit card is issued to users to enact the payment system. It allows the cardholder to access financial services in exchange for the holder's promise to pay for them later. Below are three files that contain the customer’s transaction information and inventories in the credit card information. CDW_SAPP_CUSTOMER.JSON: This file has the existing customer details. CDW_SAPP_CREDITCARD.JSON: This file contains all credit card transaction information. CDW_SAPP_BRANCH.JSON: Each branch’s information and details are recorded in this file.

Step 1: ETL proess and load the clean data into MySQL Database.

For “Credit Card System,” created a Python and PySpark SQL program to read/extract the following JSON files according to the specifications described in the mapping document.

Cleaned and transformed the data based on the requirements found in the Mapping Document.
Load the transformed Data into MySQL Database.

Step 2: Once data is loaded into the database, used front-end (console) to see/display data. For that, created a console-based Python program to satisfy System Requirements 2 (2.1 and 2.2).

2.1 Transaction Details Module
 
1)Used to display the transactions made by customers living in a given zip code for a given month and year. Order by day in descending order.
2)Used to display the number and total values of transactions for a given type.
3)Used to display the number and total values of transactions for branches in a given state.

Taken input from users and displayed relevant data.  

2.2 Customer Details Module

1) Used to check the existing account details of a customer.
2) Used to modify the existing account details of a customer.
3) Used to generate a monthly bill for a credit card number for a given month and year.
4) Used to display the transactions made by a customer between two dates. Order by year, month, and day in descending order.

Taken input from user and displayed and modified the data and wrote into database.

3 - Functional Requirements - Data analysis and Visualization

After data is loaded into the database, users can make changes from the front end, and they can also view data from the front end. The next step is to analyze and visualize the data according to the below requirements.
Used Python libraries for the below requirements:

Functional Requirements 3.1
Find and plot transactions, showing which transaction type occurs most often.
Functional Requirements 3.2
Find and plot states, showing which state has the highest number of customers. 
Functional Requirements 3.3
Find and plot the sum of all transactions for each customer, and which customer has the highest transaction amount. (First 20)
Find and plot the top three months with the largest transaction data. 
Find and plot each branches healthcare transactions, showing which branch  processed the highest total dollar value of healthcare transactions.


Overview of LOAN application Data API - PART 2
overview of the project:
Banks deal in all home loans. They have a presence across all urban, semi-urban, and rural areas. Customers first apply for a home loan; after that, a company will validate the customer's eligibility for a loan.
Banks want to automate the loan eligibility process (in real-time) based on customer details provided while filling out the online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History, and others. To automate this process, they have the task of identifying the customer segments to those who are eligible for loan amounts so that they can specifically target these customers. Here they have provided a partial dataset.

4. Functional Requirements - LOAN Application Dataset
Req-4
 Access to Loan API Endpoint
 
Functional Requirements 4.1
Create a Python program to GET (consume) data from the above API endpoint for the loan application dataset.

Functional Requirements 4.2
Find the status code of the above API endpoint.
Hint: status code could be 200, 400, 404, 401.

Functional Requirements 4.3
Once Python reads data from the API, utilized PySpark to load data into RDBMS(SQL). 

5 - Functional Requirements - Data Analysis and Visualization for Loan Application
After the data is loaded into the database, the business analyst team wants to analyze and visualize the data according to the below requirements.
Used Python libraries for the below requirements:

Req-5
Data Analysis and Visualization

Functional Requirements 5.1
Create a bar chart that shows the difference in application approvals for Married Men vs Married Women based on income ranges. (number of approvals)

Functional Requirements 5.2
Create and plot a chart that shows the difference in application approvals based on Property Area. 

CHALLENGE Requirement(Non-Graded)
Create a multi-bar plot that shows the total number of approved applications per each application demographic. 


Challenges faced: Had issues with MYSQL database not modying the records when given the UPDATE command.  Found that MYSQL had lot of process running on the background.  resolved the problem by killing unwanted processes and restarting MYSQL.

Had issues with pusing files to github using vs code.  Resolved it by using git bash to push the local git into github.




















