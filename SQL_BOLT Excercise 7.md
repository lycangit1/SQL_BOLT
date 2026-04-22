# SQLBolt Exercise 7 – Solutions

## Given Tables
- **Buildings** (building_name, capacity)  
- **Employees** (role, name, building, years_employed)

---

## 1. Find the list of all buildings that have employees

### Query:
```sql
SELECT DISTINCT building
FROM employees;
```

### Explanation:
- Retrieves unique building names from Employees table
- Only buildings with employees are included

---

## 2. Find the list of all buildings and their capacity

### Query:
```sql
SELECT building_name, capacity
FROM buildings;
```

### Explanation:
- Directly selects all buildings and their capacities
- No JOIN required

---

## 3. List all buildings and the distinct employee roles in each building (including empty buildings)

### Query:
```sql
SELECT DISTINCT b.building_name, e.role
FROM buildings b
LEFT JOIN employees e
ON b.building_name = e.building;
```

### Explanation:
- LEFT JOIN ensures all buildings are included
- DISTINCT removes duplicate role entries
- Buildings with no employees will show NULL in role column

---

## Final Combined Queries

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
