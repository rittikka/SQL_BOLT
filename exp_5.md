# <centre> Exercise 5

1. List all the Canadian cities and their populations
```sql
SELECT City, Population FROM north_american_cities WHERE COUNTRY LIKE 'CANADA';
```

2. Order all the cities in the United States by their latitude from north to south
```sql
SELECT * FROM north_american_cities 
WHERE COUNTRY = "United States"
ORDER BY latitude DESC ;
```

3. List all the cities west of Chicago, ordered from west to east
```sql
SELECT * FROM north_american_cities 
where LONGITUDE < -87.629798 
ORDER BY LONGITUDE ;
```

4. List the two largest cities in Mexico (by population)
```sql
SELECT * FROM north_american_cities
WHERE COUNTRY = "Mexico"
ORDER BY POPULATION DESC LIMIT 2 ;
```

5. List the third and fourth largest cities (by population) in the United States and their population
```sql
SELECT * FROM north_american_cities
WHERE COUNTRY = "United States"
ORDER BY POPULATION DESC LIMIT 2 OFFSET 2 ;
```