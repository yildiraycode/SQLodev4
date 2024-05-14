# SQLodev4
## sql sorguları patika odev 4 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.<br/><br/>
SELECT DISTINCT replacement_cost FROM film;<br/><br/><br/>
2.film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?<br/><br/>
SELECT count(DISTINCT replacement_cost) FROM film;<br/><br/><br/>
3.film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?<br/><br/>
SELECT count(*) FROM film<br/>
WHERE title LIKE 'T%' AND rating='G';<br/><br/><br/>
4.country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?<br/>
SELECT count(*) FROM country<br/>
WHERE length(country)=5; <br/><br/><br/>
5.city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?<br/>
SELECT COUNT(*) FROM city<br/>
WHERE city ILIKE '%R' ;<br/><br/><br/>
