# SQL_BOLT Exercise 11

## 1. Find the number of Artists in the studio (without a HAVING clause)
```sql
SELECT COUNT(*) FROM EMPLOYEES
WHERE ROLE = 'Artist';
```

## 2. Find the number of Employees of each role in the studio
```sql
SELECT ROLE, COUNT(*)
FROM EMPLOYEES
GROUP BY ROLE;
```

## 3. Find the total number of years employed by all Engineers
```sql
SELECT SUM(YEARS_EMPLOYED)
FROM EMPLOYEES
WHERE ROLE = 'Engineer';
```
