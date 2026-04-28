# SQL_BOLT Exercise 14

## 1. The director for A Bug's Life is incorrect, it was actually directed by John Lasseter
```sql
UPDATE MOVIES
SET DIRECTOR = 'John Lasseter'
WHERE TITLE = "A Bug's Life";
```

## 2. The year that Toy Story 2 was released is incorrect, it was actually released in 1999
```sql
UPDATE MOVIES
SET YEAR = 1999
WHERE TITLE = 'Toy Story 2';
```

## 3. Both the title and director for Toy Story 8 is incorrect! The title should be "Toy Story 3" and it was directed by Lee Unkrich
```sql
UPDATE MOVIES
SET TITLE = 'Toy Story 3',
DIRECTOR = 'Lee Unkrich'
WHERE TITLE = 'Toy Story 8';
```
