# SQL_BOLT Exercise 15

## 1. This database is getting too big, lets remove all movies that were released before 2005
```sql
DELETE FROM MOVIES
WHERE YEAR < 2005;
```

## 2. Andrew Stanton has also left the studio, so please remove all movies directed by him
```sql
DELETE FROM MOVIES
WHERE DIRECTOR = 'Andrew Stanton';
```
