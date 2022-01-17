# Odev10
 
#### City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
~~~sql
SELECT ci.city, co.country 
FROM city ci 
LEFT JOIN country co 
USING(country_id);
~~~
#### Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
~~~sql
SELECT c.first_name, c.last_name, p.payment_id 
FROM customer c 
RIGHT JOIN payment p 
USING(customer_id);
~~~
#### Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
~~~sql
SELECT c.first_name, c.last_name, r.rental_id 
FROM customer c 
FULL JOIN rental r 
USING(customer_id);
~~~