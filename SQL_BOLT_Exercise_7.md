# SQL_BOLT Exercise 7 – Solutions

## 1
```sql
SELECT DISTINCT building
FROM employees;
```

## 2
```sql
SELECT building_name, capacity
FROM buildings;
```

## 3
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
