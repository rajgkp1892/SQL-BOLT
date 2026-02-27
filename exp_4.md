
# Exercise 4 — SQL Queries for Pixar Movies

This file contains all the SQL queries for Exercise 4 tasks on Pixar movies.

---

## **Task 1: List all directors alphabetically, without duplicates**
```sql
SELECT DISTINCT director
FROM pixar_movies
ORDER BY director ASC;
```
## **Task 2: List the last four Pixar movies released (most recent first) ** 
```sql
SELECT title, release_year
FROM pixar_movies
ORDER BY release_year DESC
LIMIT 4;

```
 ## Task 3: List the first five Pixar movies sorted alphabetically
```sql
SELECT title, release_year
FROM pixar_movies
ORDER BY title ASC
LIMIT 5;

```
Task 4: List the next five Pixar movies sorted alphabetically
```
SELECT title, release_year
FROM pixar_movies
ORDER BY title ASC
LIMIT 5 OFFSET 5;
```
