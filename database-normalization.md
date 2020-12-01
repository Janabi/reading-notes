# Database Normalization
## What does database normalization mean?

***Database Normalization*** means that we are going to create a database table of fixed columns and changeable rows for a single purposes.

Therefore, there is no need to build up a single table with multiple purposes which it will end up really hard to insert, select, delete or even update any certain rows.

Lets take a look for this following table which includes a **salesperson information** and their **customers**.
![figure1](https://www.essentialsql.com/wp-content/uploads/2014/06/FirstNormalFormUnormalized-1.png)
![figure2](https://www.essentialsql.com/wp-content/uploads/2014/06/Intro-Deletion-Anomaly-e1425554658757.png)

As you can see the figures above, the table has three purposes where we can separate them into three tables as follows:
1. Information of salesperson.

EmployeeID#| SalesPerson         |SalesOffice             |Customers
-----------|---------------------|------------------------|-------------
1          |Abdulrahman          |Amman                   |Mersedes

2. The offices location and contact info.

ID#        | Location            |ContactOffice             
-----------|---------------------|------------------------
1          |Amman                |065554444

3. 3The customer and their contacts info.

ID#        | Customers           |ContactOffice             
-----------|---------------------|------------------------
1          |Mersedes             |065554433

***The reference of this markdown from the following [link](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/).***