1.	country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.
2.	country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
3.	film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
4.	film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.

1.	Soru cevabı
select country
from country
where country LIKE 'A%a'

2.	Soru cevabı 
select country
from country
WHERE LENGTH(country) >= 6 AND country LIKE '%n';

3.	 soru cevabı 
select title
from film
where title ILIKE '%T%T%T%T%'

4.	Soru cevabı 
select *
from film
where rental_rate = 2.99 and title like 'C%'and length > 90
