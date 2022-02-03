Problem 1: Revising Aggregations - The COUNT function
Query a count of the number of cities in CITY having a Population larger than 100000.

Solution:
SELECT COUNT(DISTINCT(NAME)) FROM CITY
WHERE POPULATION > 100000


Problem 2: Revising Aggregations - The COUNT function
Query the total population of all cities in CITY where District is California.

Solution:
SELECT SUM(POPULATION) FROM CITY
WHERE DISTRICT = "California"


Problem 3: Revising Aggregations - Averages
Query the average population of all cities in CITY where District is California.

Solution:
SELECT AVG(POPULATION) FROM CITY
WHERE DISTRICT = "California";


Problem 4: Average Population
Query the average population for all cities in CITY, rounded down to the nearest integer.

Solution:
SELECT ROUND(AVG(POPULATION)) FROM CITY;


Problem 5: Japan Population
Query the sum of the populations for all Japanese cities in CITY. The COUNTRYCODE for Japan is JPN.

Solution:
SELECT SUM(POPULATION) FROM CITY
WHERE COUNTRYCODE = 'JPN';


Problem 6: Population Density Difference
Query the difference between the maximum and minimum populations in CITY.

Solution:
SELECT MAX(POPULATION) - MIN(POPULATION) FROM CITY;

Problem 7: 
