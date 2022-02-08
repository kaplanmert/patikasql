## test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

CREATE TABLE test (
      id INTEGER,
      name VARCHAR(50),
      birthday DATE,
      email VARCHAR(100)
);

## Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

UPDATE test 
SET name = 'mert', birthday = '1998-07-04', email='laylay@laylay.com'
WHERE id BETWEEN 3 AND 7
RETURNING *;

## Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
Delete from TEST where id between 3 and 7 returning *;
