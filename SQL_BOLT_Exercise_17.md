# SQL_BOLT Exercise 17

## 1. Add a column named Aspect_ratio with a FLOAT data type
```sql
ALTER TABLE MOVIES
ADD COLUMN ASPECT_RATIO FLOAT;
```

## 2. Add another column named Language with a TEXT data type and default value English
```sql
ALTER TABLE MOVIES
ADD COLUMN LANGUAGE TEXT DEFAULT 'English';
```
