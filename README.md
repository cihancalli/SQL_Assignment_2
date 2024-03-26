# SQL_Assignment_2

## Sorgu Senaryoları

* Film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız (BETWEEN - AND yapısını kullanınız.)

```bash
SELECT *
FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99
ORDER BY replacement_cost ASC;
```

* Actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. (IN operatörünü kullanınız.)

```bash
SELECT first_name, last_name
FROM actor
WHERE first_name IN ('Penelope', 'Nick', 'Ed')
ORDER BY first_name ASC;
```

* Film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. (IN operatörünü kullanınız.)

```bash
SELECT *
FROM film
WHERE rental_rate IN (0.99, 2.99, 4.99)
AND replacement_cost IN (12.99, 15.99, 28.99)
ORDER BY rental_rate ASC, replacement_cost ASC;
```


## Notlar :

* Bu sorgular, dvdrental örnek veri tabanı üzerinde çalıştırılmalıdır.
* Sorgular, MySQL dilinde yazılmıştır.
* BETWEEN operatörü, bir aralıktaki değerleri seçmek için kullanılır.
* IN operatörü, bir listedeki değerleri seçmek için kullanılır.
* ORDER BY sorgusu, sonuçları belirli bir sütuna göre sıralamak için kullanılır.

## Ek Bilgiler :
* MySQL sorguları hakkında daha fazla bilgi için MySQL Eğitimi: URL MySQL Eğitimi kaynaklarına bakabilirsiniz.
* dvdrental örnek veri tabanı hakkında daha fazla bilgi için MySQL Örnek Veri Tabanları: URL MySQL Örnek Veri Tabanları sayfasına bakabilirsiniz.
