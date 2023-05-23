# SQL_ODEV4
## SQL Ödev 4 | DISTINCT and COUNT

1- ) film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
SELECT DISTINCT replacement_cost FROM film;


#### "replacement_cost"
19.99
25.99
13.99
10.99
23.99
18.99
20.99
24.99
11.99
15.99
27.99
29.99
12.99
14.99
22.99
16.99
28.99
9.99
17.99
21.99
26.99

2- ) film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?


SELECT COUNT (DISTINCT replacement_cost) FROM film;

#### "count" = 21

3- ) film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

SELECT COUNT(*) FROM film 
WHERE title LIKE 'T%' AND rating = 'G';

#### "count" = 9

4- ) country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

SELECT COUNT(DISTINCT country) FROM country 
WHERE country like '_____';
#### "count" = 9
5- )city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?


SELECT COUNT(city) FROM city 
WHERE city ILIKE 'R%'

#### "count" = 13
