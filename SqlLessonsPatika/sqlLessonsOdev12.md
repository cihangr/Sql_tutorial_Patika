
1. **film** tablosunda **film** uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama **film** uzunluğundan fazla kaç tane **film** vardır?
```
SELECT COUNT(length) FROM film
WHERE length > ANY
(SELECT AVG(length) FROM film);
```
2. **film** tablosunda en yüksek **rental_rate** değerine sahip kaç tane **film** vardır?
```
SELECT COUNT(rental_rate) FROM film
WHERE rental_rate = ANY
(SELECT MAX(rental_rate) FROM film);
```
3. **film** tablosunda en düşük **rental_rate** ve en düşün **replacement_cost** değerlerine sahip **film**leri sıralayınız.
```
SELECT rental_rate, replacement_cost FROM film
WHERE rental_rate = ALL
(SELECT MIN(rental_rate) FROM film)
AND replacement_cost = ALL
(SELECT MIN(replacement_cost) FROM film);
```
4. **payment** tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.
```
SELECT customer_id FROM payment
GROUP BY customer_id
HAVING COUNT(customer_id) =
(
	SELECT COUNT(customer_id) FROM payment
	GROUP BY customer_id
	ORDER BY COUNT(customer_id) DESC
	LIMIT 1
);
```

My Patika account [Patika](https://academy.patika.dev/profile)

My Linkedin account [Linkedin](https://www.linkedin.com/in/cihangr/)

My GitHub account [GitHub](https://github.com/cihangr)