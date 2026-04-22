# SQL_BOLT Exercise 8 – Solutions

## 1. Find the name and role of all employees who have not been assigned to a building
```sql
SELECT name, role
FROM employees
WHERE building IS NULL;
```

## 2. Find the names of the buildings that hold no employees
```sql
SELECT b.building_name
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building
WHERE e.building IS NULL;
```

## Final Queries
```sql
-- 1
SELECT name, role
FROM employees
WHERE building IS NULL;

-- 2
SELECT b.building_name
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building
WHERE e.building IS NULL;
```
