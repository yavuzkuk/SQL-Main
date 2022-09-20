# SQL-10

### (Left ve Right olan kümeleri seçmek size kalmış)

- city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.


`
SELECT country.country ,city.city FROM country
LEFT JOIN city ON  city.country_id = country.country_id
`

- customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.

`
SELECT payment.payment_id , customer.first_name , customer.last_name FROM payment
RIGHT JOIN customer ON customer.customer_id = payment.customer_id
`


- customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.


`
SELECT customer.first_name , customer.last_name , rental.rental_id FROM customer
FULL JOIN rental ON customer.customer_id = rental.customer_id
`

