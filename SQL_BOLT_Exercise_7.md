# SQL_BOLT Exercise 7 – Solutions

## 1. Find the list of all buildings that have employees
```sql
SELECT DISTINCT building
FROM employees;
```

## 2. Find the list of all buildings and their capacity
```sql
SELECT building_name, capacity
FROM buildings;
```

## 3. List all buildings and the distinct employee roles in each building (including empty buildings)
```sql
SELECT DISTINCT b.building_name, e.role
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building;
```

## Final Queries
```sql
-- 1
SELECT DISTINCT building
FROM employees;

-- 2
SELECT building_name, capacity
FROM buildings;

-- 3
SELECT DISTINCT b.building_name, e.role
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building;
```
