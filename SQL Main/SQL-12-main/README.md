# SQL-12


- film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

`
SELECT COUNT(*) FROM film
WHERE length > 
(
SELECT AVG(length) FROM film
)
`


- film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

`
SELECT COUNT(*) FROM film
WHERE rental_rate =
(
  SELECT MAX(rental_rate) FROM film
)
`

- film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.

`
SELECT title FROM film
WHERE rental_rate =
(
SELECT rental_rate FROM film
WHERE MIN(rental_rate)
)
AND
replacement_cost =
(
SELECT replacement_cost FROM film
WHERE MIN(replacement_cost)
)
`

- payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

`
SELECT COUNT(payment_id), (customer_id) FROM payment
GROUP BY customer_id
ORDER BY COUNT(payment_id) DESC
`



