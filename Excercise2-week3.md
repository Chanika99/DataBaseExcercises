#Week3-Excercise 2

Nape Vithanage Chanika Anjalee

###Question 1 

select * from goal;
![Q1-Ex2.png](Q1-Ex2.png)

###Question 2

select name, type from airport where iso_country="FI";
![Q2-Ex2.png](Q2-Ex2.png)

###Question 3

select name from airport where iso_country="FI" oder by name asc;
![Q3-Ex2.png](Q3-Ex2.png)

###Question 4

select name, type from airport where iso_country="FI" oder by type asc,name asc;
![Q4 -Ex2.png](Q4%20-Ex2.png)

###Question 5

select name from country where name like "F%";
![Q5-Ex2.png](Q5-Ex2.png)

###Question 6

select name from country where name like "%F%";
![Q6-Ex2.png](Q6-Ex2.png)

###Question 7

select location from game where screen_name="Vesa";
![Q7-Ex2.png](Q7-Ex2.png)

###Question 8

select co2_consumed from game where screen_name="Ilkka";
![Q8-Ex2.png](Q8-Ex2.png)

###Question 9

select DISTINCT co2_budget from game;
![Q9-Ex2.png](Q9-Ex2.png)

###Question 10

select screen_name, co2_budget, co2_consumed, co2_budget - co2_consumed as co2_left from game where screen_name="Ilkka";
![Q10-Ex2.png](Q10-Ex2.png)