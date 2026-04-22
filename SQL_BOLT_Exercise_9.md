# SQL_BOLT Exercise 9 – Solutions

## 1. List all movies and their combined sales in millions of dollars
```sql
SELECT m.title, (b.domestic_sales + b.international_sales)/1000000 AS total_sales_millions
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;
```

## 2. List all movies and their ratings in percent
```sql
SELECT m.title, b.rating * 10 AS rating_percent
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;
```

## 3. List all movies that were released on even number years
```sql
SELECT *
FROM movies
WHERE year % 2 = 0;
```

## Final Queries
```sql
-- 1
SELECT m.title, (b.domestic_sales + b.international_sales)/1000000 AS total_sales_millions
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;

-- 2
SELECT m.title, b.rating * 10 AS rating_percent
FROM movies m
JOIN boxoffice b
ON m.id = b.movie_id;

-- 3
SELECT *
FROM movies
WHERE year % 2 = 0;
```
