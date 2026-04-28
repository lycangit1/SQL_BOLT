# SQL_BOLT Exercise 10

## 1. Find the longest time that an employee has been at the studio
```sql
SELECT MAX(YEARS_EMPLOYED) FROM EMPLOYEES;
```

## 2. For each role, find the average number of years employed by employees in that role
```sql
SELECT ROLE, AVG(YEARS_EMPLOYED)
FROM EMPLOYEES
GROUP BY ROLE;
```

## 3. Find the total number of employee years worked in each building
```sql
SELECT BUILDING, SUM(YEARS_EMPLOYED)
FROM EMPLOYEES
GROUP BY BUILDING;
```
