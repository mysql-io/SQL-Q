# SQL-Q
***
Question. How to find Nth highest salary from a table ?

Answer.
```SQL
SELECT * FROM (SELECT DENSE_RANK() OVER (ORDER BY SALARY DESC) AS densRank,firstname,Salary FROM Employee ) AS Maxs WHERE densRank = 3
```
***
