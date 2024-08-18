# PostgreSQL Queries - Patika.dev ASP.NET Core Assignment

This repository contains SQL queries related to the PostgreSQL database as part of the assignment for the Patika.dev ASP.NET Core course. The queries are designed to perform various operations on the `film`, `country`, and `city` tables of a sample database.

## Queries Overview

### 1. Retrieve distinct values from the `replacement_cost` column in the `film` table
```sql
SELECT DISTINCT replacement_cost FROM film;
```
This query selects distinct values from the replacement_cost column in the film table.

### 2. Count the number of distinct values in the replacement_cost column in the film table
```sql

SELECT COUNT(DISTINCT replacement_cost) FROM film;
```
This query counts the number of distinct values in the replacement_cost column in the film table.

### 3. Count the number of film titles that start with 'T' and have a rating of 'G'
```sql

SELECT COUNT(*) FROM film 
WHERE title LIKE 'T%' 
AND rating = 'G';
```
This query counts the number of films in the film table where the title starts with 'T' and the rating is 'G'.

### 4. Count the number of country names that are 5 characters long
```sql

SELECT COUNT(*) FROM country
WHERE LENGTH(country) = 5;
```
This query counts the number of country names in the country table that are exactly 5 characters long.

### 5. Count the number of city names that end with 'R' or 'r'
```sql

SELECT COUNT(*) FROM city 
WHERE city ILIKE '%R';
```
This query counts the number of city names in the city table that end with 'R' or 'r', case insensitive.
