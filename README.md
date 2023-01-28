AŞAĞIDAKİ SORGU SENARYOLARINI DVDRENTAL ÖRNEK VERİ TABANI ÜZERİNDEN GERÇEKLEŞTİRİNİZ.
1.	Film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.
SELECT title,description FROM film;
2.	Film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük ve 75 ten küçük olma koşullarıyla sıralayınız.
SELECT * FROM film
WHERE length > 60 AND length<75
3.	Film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 ve replacement_cost 12.99 veya 28.99 olma koşullarıyla sıralayınız.
SELECT * FROM film 
WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR rental_rate = 28.99);
4.	Customer tablosunda bulunan first_name sütunundaki değeri 'mary' olan müşterinin last_name sütunundaki değeri nedir?
SELECT * FROM customer
WHERE first_name = 'Mary'; 'Mary' olan müşterinin last_name sütunundaki değeri = ‘Smith’
5.	Film tablosundaki uzunluğu(length) 50 ten büyük olmayıp aynı zamanda rental_rate değeri 2.99 veya 4.99 olmayan verileri sıralayınız.
SELECT * FROM film
WHERE length < 50 AND NOT  (rental_rate = 2.99 OR rental_rate = 4.99);

