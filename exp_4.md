# <centre> Exercise 4
1. List all directors of Pixar movies (alphabetically), without duplicates
```sql
SELECT DISTINCT director FROM movies ORDER BY DIRECTOR;
```

2. List the last four Pixar movies released (ordered from most recent to least)
```sql
SELECT * FROM MOVIES ORDER BY YEAR DESC LIMIT 4;
```

3. List the first five Pixar movies sorted alphabetically
```sql
SELECT * FROM MOVIES ORDER BY TITLE LIMIT 5;
```

4. List the next five Pixar movies sorted alphabetically
```sql
SELECT * FROM MOVIES ORDER BY TITLE LIMIT 5 OFFSET 5;
```