# homework_submission-
full test

#1. Weather Observation Station 13

Submitted Code

select round(sum(LAT_N),4) from station where LAT_N > 38.7880 and LAT_N < 137.2345;

#2. Revising the Select Query I

Submitted Code

select * from CITY where countrycode = 'USA' and population > 100000

#3. Revising the Select Query II

Submitted Code

select name from CITY where countrycode = 'USA' and population > 120000

#4. Japanese Cities' Names

Submitted Code

select name from city where countrycode = "JPN"

#5. Select All 

Submitted Code

select * from city

#6. Select By ID

Submitted Code

select * from CITY where id = 1661

#7. Japanese Cities' Attributes

Submitted Code

select * from city where countrycode = 'JPN'

#8. Weather Observation Station 1

Submitted Code

select city, state from station

#9. Employee Names

Submitted Code

select name from employee order by name asc

#10. Weather Observation Station 3

Submitted Code

select distinct city from station where id % 2 = 0

#11. Revising Aggregations - The Count Function

Submitted Code

select count(name) from CITY where population > 100000

#12. Revising Aggregations - The Sum Function

Submitted Code

select sum(population) from CITY where district = "California"

#13. Weather Observation Station 5

Submitted Code

Select City,char_LENGTH(City) from Station Order By Length(City), City asc limit 1; Select City,char_LENGTH(City) from Station Order By Length(City) desc, City desc limit 1;

#14. Weather Observation Station 8

Submitted Code 

select distinct city from station where left(city,1) in ('a','e','i','o','u') and right(city, 1) in ('a','e','i','o','u')

#15. Weather Observation Station 6 

Submitted Code 

select distinct(city) from station where left(city,1) in ('a','e','i','o','u')

#16. African Cities 
 
Submitted Code 

select city.name from CITY inner join COUNTRY on CITY.CountryCode = COUNTRY.Code where continent = 'Africa'

#17. Revising Aggregations - Averages 

Submitted Code 

select avg(population) from city where district = 'California'

#18. Higher Than 75 Marks 

Submitted Code 

SELECT NAME FROM STUDENTS WHERE MARKS > 75 ORDER BY RIGHT(NAME, 3), ID ASC;

#19. Weather Observation Station 2 

Submitted Code 

select round(sum(LAT_N),2), round(sum(LONG_w),2) from station

#20. Average Population of Each Continent 

Submitted Code 

select country.continent, floor(avg(city.population)) from city inner join country on CITY.CountryCode = COUNTRY.Code group by continent;

#21.Weather Observation Station 15 

Submitted Code 

select round(LONG_W,4) from station where LAT_N = (select max(LAT_N) from station where LAT_N < 137.2345)

#22. Weather Observation Station 11

Submitted Code 

select distinct(city) from station where left(city,1) not in ('a','i','u','o','e') or right(city, 1) not in ('a','i','u','o','e')

#23. Weather Observation Station 12

Submitted Code 

select distinct(city) from station where left(city,1) not in ('a','e','i','u','o') and right(city, 1) not in ('a','e','i','u','o')

#24. Asian Population 

Submitted Code 

select sum(city.population) from city inner join country on city.countrycode = country.code where continent = 'Asia'

#25. Average Population 

Submitted Code 

select round(avg(population)) from city

#26. Weather Observation Station 14 

Submitted Code 

select truncate(max(LAT_N),4) from station where LAT_N < 137.2345

#27. Weather Observation Station 17 

Submitted Code

select round(LONG_W,4) from station where (LAT_N) = (select MIN(LAT_N) from station where LAT_N > 38.7780)

#28. Weather Observation Station 16 

Submitted Code

select round(min(LAT_N),4) from station where LAT_N > 38.7780

#29. The Blunder 

Submitted Code

select ceil(avg(salary) - avg(replace(salary,'0',''))) from EMPLOYEES;

#30. Employee Salaries

Submitted Code

select name from Employee where salary > 2000 and months < 10 order by employee_id asc

#31. Population Density Difference

Submitted Code

select max(population) - min(population) as difference from city

#32. Japan Population

Submitted Code

select sum(population) from city where countrycode = 'JPN'

#33. Weather Observation Station 10

Submitted Code

select distinct(city) from station where right(city,1) not in ('a','i','e','u','o')

#34. Weather Observation Station 9

Submitted Code

select distinct(city) from station where left(city,1) not in ('a','i','e','u','o')

#35. Weather Observation Station 7

Submitted Code

select distinct city from station where right(city,1) in ('a','e','i','u','o')

#36. Draw The Triangle 1

Submitted Code

set @h:= 21; SELECT REPEAT('* ', @h:= @h - 1) FROM information_schema.tables

#37. Type of Triangle 

Submitted Code

SELECT  
case 
WHEN A + B <= C or A + C <= B or B + C <= A then 'Not A Triangle'
WHEN A = B and B = C THEN 'Equilateral' 
WHEN A = B OR B = C OR A = C THEN 'Isosceles' 
else 'Scalene'
END as sad FROM TRIANGLES;

#38. Top Earners 

Submitted Code

select (salary*months) as earnings, count(*) from employee group by earnings order by earnings desc limit 1 

#39. Weather Observation Station 4

Submitted Code

select count(city) - count(distinct city) from station 




