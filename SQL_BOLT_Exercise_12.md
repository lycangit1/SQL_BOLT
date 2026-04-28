# SQL_BOLT Exercise 12

## 1. Find the number of movies each director has directed
```sql
SELECT DIRECTOR, COUNT(*)
FROM MOVIES
GROUP BY DIRECTOR;
```

## 2. Find the total domestic and international sales that can be attributed to each director
```sql
SELECT M.DIRECTOR,
SUM(B.DOMESTIC_SALES) AS TOTAL_DOMESTIC_SALES,
SUM(B.INTERNATIONAL_SALES) AS TOTAL_INTERNATIONAL_SALES
FROM MOVIES M
JOIN BOXOFFICE B
ON M.ID = B.MOVIE_ID
GROUP BY M.DIRECTOR;
```
