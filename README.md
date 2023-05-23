# SQL_ODEV4
## SQL Ödev 4 | DISTINCT and COUNT

1- ) film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
SELECT DISTINCT replacement_cost FROM film;


#### "replacement_cost"
1) 19.99-
2) 25.99
3) 13.99
4) 10.99
5) 23.99
6) 18.99
7) 20.99
8) 24.99
9) 11.99
10)15.99
11) 27.99
12) 29.99
13) 12.99
14) 14.99
15) 22.99
16) 16.99
17) 28.99
18) 9.99
19) 17.99
20) 21.99
21) 26.99

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
