# SQL Exercise 2 – Filtering Records

## Objective
Practice SQL filtering using `WHERE`, `BETWEEN`, `NOT BETWEEN`, `ORDER BY`, and `LIMIT` on the `movies` table.

---

## Queries

1️⃣ Find the movie with a row id of 6  
```sql
SELECT * FROM movies
WHERE id = 6;


2️⃣ Find the movies released in the years between 2000 and 2010
SELECT * 
FROM Film
WHERE year BETWEEN 2000 AND 2010;
3️⃣ Find the movies NOT released in the years between 2000 and 2010
SELECT * 
FROM Film
WHERE year NOT BETWEEN 2000 AND 2010;
4️⃣ Find the first 5 Pixar movies and their release year
SELECT title, year 
FROM Film
WHERE studio = 'Pixar'
ORDER BY year ASC
LIMIT 5;
