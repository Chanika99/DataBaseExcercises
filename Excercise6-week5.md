#Week5-Excercise 6

Nape Vithanage Chanika Anjalee

###Question 1 

select max(elevation_ft) from airport;
![Q1-Ex6.png](Q1-Ex6.png)

###Question 2

select continent, count(*) from country group by continent;
![Q2-Ex6.png](Q2-Ex6.png)

###Question 3

select screen_name, count(*) from game, goal_reached where id = game_id group by screen_name;
![Q3-Ex6.png](Q3-Ex6.png)

###Question 4

select screen_name from game where co2_consumed in(select min(co2_consumed) from game );
![Q4-Ex6.png](Q4-Ex6.png)

###Question 5

select country.name, count(*) from airport, country where airport.iso_country = country.iso_country group by country.iso_country order by count(*) desc limit 50;
 ![Q5-Ex6.png](Q5-Ex6.png)

###Question 6

select country.name from airport, country where airport.iso_country = country.iso_country group by country.iso_country having count(*) > 1000;
![Q6-Ex6.png](Q6-Ex6.png)

###Question 7

select name from airport where elevation_ft in ( select max(elevation_ft) from airport );
![Q7-Ex6.png](Q7-Ex6.png)

###Question 8

select name from country where iso_country in ( select iso_country from airport where elevation_ft in( select max(elevation_ft) from airport ) );
![Q8-Ex6.png](Q8-Ex6.png)

###Question 9

select count(*) from game, goal_reached where id = game_id and screen_name = "Vesa" group by screen_name;
![Q9-Ex6.png](Q9-Ex6.png)

###Question 10

select name from airport where latitude_deg in( select min(latitude_deg) from airport );
![Q10-Ex6.png](Q10-Ex6.png)