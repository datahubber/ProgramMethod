SELECT * FROM CITY WHERE CountryCode = "USA" and POPULATION > 100000;  
SELECT NAME FROM CITY WHERE CountryCode = "USA" and POPULATION > 120000;  
SELECT * FROM CITY;  
SELECT * FROM CITY WHERE ID = 1661;  
SELECT * FROM CITY WHERE COUNTRYCODE = 'JPN';  
SELECT NAME FROM CITY WHERE COUNTRYCODE = 'JPN';  
SELECT CITY, STATE FROM STATION;  
SELECT DISTINCT CITY FROM STATION WHERE ID % 2 = 0;  
SELECT (COUNT(CITY) - COUNT(DISTINCT CITY)) FROM STATION;  
SELECT CITY, LENGTH(CITY) AS name_length FROM STATION ORDER BY name_length, CITY LIMIT 1;  
SELECT CITY, LENGTH(CITY) AS name_length FROM STATION ORDER BY name_length DESC, CITY LIMIT 1;  
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[aeiouAEIOU]';  
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '[aeiouAEIOU]$';  
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[aeiouAEIOU]' AND CITY REGEXP '[aeiouAEIOU]$';  
SELECT DISTINCT CITY FROM STATION WHERE NOT CITY REGEXP '^[AEIOUaeiou]';  
SELECT DISTINCT CITY FROM STATION WHERE NOT CITY REGEXP '[AEIOUaeiou]$';  
SELECT product_id FROM Products WHERE low_fats = 'Y' AND recyclable = 'Y';  
SELECT name FROM Customer WHERE referee_id IS NULL OR referee_id <> 2;  
SELECT name, population, area FROM World WHERE area >= 3000000 OR population >= 25000000;  
SELECT DISTINCT author_id AS id FROM Views WHERE author_id = viewer_id ORDER BY id;  
SELECT tweet_id FROM Tweets WHERE length(content) > 15;  
