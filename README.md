# SQL-Q
***
Question. What are the different types of SQL’s statements? 

Answer.
```SQL
1. DQL - Data Query Language ( or) Data Retrival Language 

SELECT Statement 
2. DML – Data Manipulation Language
    DML is used for manipulation of the data itself.

INSERT Statement
UPDATE Statement
DELETE Statement
3. DDL – Data Definition Language
    DDL is used to define the structure that holds the data. 

CREATE Statement
ALTER Statement
DROP Statement
RENAME Statement
TRUNCATE Statement
4. DCL – Data Control Language 
    DCL is used to control the visibility of data.

GRANT Statement
REVOKE Statement
5. TCL - Transaction Control Language

COMMIT Statement
ROLLBACK Statement
SAVEPOINT Statement
```
***

***
Question. How to find Nth highest salary from a table ?

Answer.
```SQL
SELECT * FROM (SELECT DENSE_RANK() OVER (ORDER BY SALARY DESC) AS densRank,firstname,Salary FROM Employee ) AS Maxs WHERE densRank = 3
```
***
