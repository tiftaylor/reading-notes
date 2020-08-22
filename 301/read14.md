# Read:14 \| DB Normalization
Article: [Database Normalization Explained](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)     

## Notes from Article: 

> **Database Normalization** is basically organizing a database of information into tables and columns with a single purpose. 

- Using a 1 purpose table design, you reduce duplicate data in your database
- As tables satisfy successive db normalization forms, they are less prone to **modification anamolies**
- You want to use Database Normalization because: 
  - minimize duplicate data
  - minimize modification issues
  - simplify query searches
- Data Duplication leads to inscreased storage and descreases performance

### Let's use this table as an example for Modification Issues: 

<image src="../images/read14.png" style="width: 400px">

- Modification Anomalies make data difficult to maintain when there are changes
  - Insert Anomaly Ex: We can't record a new sales office until we know the sales person because the primary key is based on Employee ID
  - Update Anomaly Ex: If the office number changes then we have to make multiple updates instead of one. And if we don't catch all we will have *inconsistencies* :(
  - Deletion Anomaly Ex: If John retires and we delete his row, we lose info about the NY officce

- This is why it's important to have tables serve a single purpose

### Common form of DB Normalization is 1NF, 2NF, 3NF
  - i.e. The forms are progressive so to qualify for 3rd normal form, a table must satisfy the rules for 2nd normal form, etc. 
  - Below is a screenshot representing the defintion of the 3 Normal Forms: 
    - <image src="../images/read14-1.png" style="width: 400px">





[Back to Home](README.md)