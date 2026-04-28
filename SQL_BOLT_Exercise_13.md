# SQL_BOLT Exercise 13

## 1. Add the studio's new production, Toy Story 4, to the list of movies (you can use any director)
```sql
INSERT INTO MOVIES (ID, TITLE, DIRECTOR, YEAR, LENGTH_MINUTES)
VALUES (15, 'Toy Story 4', 'John Lasseter', 2019, 100);
```

## 2. Add the record to the BoxOffice table
```sql
INSERT INTO BOXOFFICE (MOVIE_ID, RATING, DOMESTIC_SALES, INTERNATIONAL_SALES)
VALUES (15, 8.7, 340000000, 270000000);
```
