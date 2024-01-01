1. **film** tablosundan 'K' karakteri ile başlayan en uzun ve replacenet_cost u en düşük 4 **film**i sıralayınız.
```
SELECT length, replacement_cost FROM film
WHERE title ILIKE 'k%'
ORDER BY length DESC, replacement_cost ASC
LIMIT 4;
```
2. **film** tablosunda içerisinden en fazla sayıda **film** bulunduran rating kategorisi hangisidir?
```
SELECT count(*), rating FROM film
GROUP BY rating
ORDER BY count(*) DESC
LIMIT 1;
```
3. **customer** tablosunda en çok alışveriş yapan müşterinin adı nedir?
```
SELECT customer.first_name, customer.last_name, SUM(payment.amount) AS amount FROM customer
JOIN payment ON customer.customer_id = payment.customer_id
GROUP BY customer.customer_id, customer.first_name, customer.last_name
ORDER BY SUM(payment.amount) DESC
LIMIT 1;
```
4. **category** tablosundan kategori isimlerini ve kategori başına düşen **film** sayılarını sıralayınız.
```
SELECT category.name, COUNT(*) FROM category
JOIN film_category ON category.category_id = film_category.category_id
JOIN film ON film_category.film_id = film.film_id
GROUP BY category.name
ORDER BY COUNT(film.film_id) DESC;
```
5. **film** tablosunda isminde en az 4 adet 'e' veya 'E' karakteri bulunan kç tane **film** vardır?
```
SELECT COUNT(title) FROM film
WHERE title ILIKE '%e%e%e%e%';
```

My Patika account [Patika](https://academy.patika.dev/profile)

My Linkedin account [Linkedin](https://www.linkedin.com/in/cihangr/)

My GitHub account [GitHub](https://github.com/cihangr)