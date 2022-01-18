# Odev9

#### City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
~~~sql
SELECT ci.city, co.country 
FROM city ci 
JOIN country co 
USING(country_id);
~~~
#### Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
~~~sql
SELECT c.first_name, c.last_name, p.payment_id 
FROM customer c 
JOIN payment p 
USING(customer_id);
~~~
#### Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
~~~sql
SELECT c.first_name, c.last_name, r.rental_id 
FROM customer c 
JOIN rental r 
USING(customer_id);
~~~