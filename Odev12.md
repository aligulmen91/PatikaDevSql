# Odev12

#### Film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
~~~sql
SELECT COUNT(*) 
FROM film 
WHERE length > ( SELECT AVG(length) FROM film);
~~~

#### Film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
~~~sql
SELECT COUNT(*) 
FROM film 
WHERE rental_rate = ( SELECT MAX(rental_rate) FROM film);
~~~

#### Film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
~~~sql
SELECT *
FROM film
WHERE film_id = ANY
( SELECT film_id
 FROM film
WHERE rental_rate = ( SELECT MIN(rental_rate ) FROM film )
 AND
 replacement_cost = ( SELECT MIN(replacement_cost) FROM film ) );
~~~

#### Payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.
~~~sql
SELECT *
FROM customer c
JOIN payment p
USING ( customer_id )
WHERE amount = ( SELECT MAX(amount) from payment );
~~~