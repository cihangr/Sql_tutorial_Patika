1. **test** veritabanınızda **employee** isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```
CREATE TABLE employee (
	id INT NOT NULL,
	name VARCHAR(50) NOT NULL,
	birthday DATE NOT NULL,
	email VARCHAR(100)
);
```
2. Oluşturduğumuz **employee** tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```
insert into employee (id, name, birthday, email) values (1, 'Carmine', '7/20/1988', 'cknaggs0@cargocollective.com');
insert into employee (id, name, birthday, email) values (2, 'Chic', '9/21/1981', 'cabthorpe1@wordpress.com');
insert into employee (id, name, birthday, email) values (3, 'Tabitha', '5/20/1983', 'tkearey2@1688.com');
insert into employee (id, name, birthday, email) values (4, 'Laurens', '6/6/1996', null);
insert into employee (id, name, birthday, email) values (5, 'Madeline', '7/19/2008', 'mwalklate4@hhs.gov');
insert into employee (id, name, birthday, email) values (6, 'Jarib', '11/8/1984', null);
insert into employee (id, name, birthday, email) values (7, 'Benoit', '5/15/1967', 'bhewkin6@tinypic.com');
insert into employee (id, name, birthday, email) values (8, 'Maryrose', '1/29/1977', 'msimmonite7@theatlantic.com');
insert into employee (id, name, birthday, email) values (9, 'Yoshiko', '1/12/1989', null);
insert into employee (id, name, birthday, email) values (10, 'Anne-marie', '11/29/2003', 'ajessen9@bravesites.com');
insert into employee (id, name, birthday, email) values (11, 'Donnamarie', '10/17/1994', null);
insert into employee (id, name, birthday, email) values (12, 'Zolly', '5/16/2007', 'zhamorb@gov.uk');
insert into employee (id, name, birthday, email) values (13, 'Vinson', '4/28/1987', 'varchbuttc@skype.com');
insert into employee (id, name, birthday, email) values (14, 'Batsheva', '11/2/1996', 'borkneyd@businesswire.com');
insert into employee (id, name, birthday, email) values (15, 'Amata', '5/11/2009', null);
insert into employee (id, name, birthday, email) values (16, 'Katey', '9/1/1974', 'kbloyf@netvibes.com');
insert into employee (id, name, birthday, email) values (17, 'Karina', '9/14/1992', null);
insert into employee (id, name, birthday, email) values (18, 'Karlene', '4/11/2001', 'kgeggh@bbb.org');
insert into employee (id, name, birthday, email) values (19, 'Ambrosi', '9/5/1988', 'adeclercqi@apple.com');
insert into employee (id, name, birthday, email) values (20, 'Rosmunda', '5/15/1973', 'raddeycottj@infoseek.co.jp');
insert into employee (id, name, birthday, email) values (21, 'Fredra', '6/11/1973', null);
insert into employee (id, name, birthday, email) values (22, 'Brodie', '6/19/1975', 'blahrsl@earthlink.net');
insert into employee (id, name, birthday, email) values (23, 'Peggy', '9/18/1997', 'phaburnem@twitpic.com');
insert into employee (id, name, birthday, email) values (24, 'Yvor', '6/9/1984', 'ybernoletn@sina.com.cn');
insert into employee (id, name, birthday, email) values (25, 'Karly', '10/6/1978', null);
insert into employee (id, name, birthday, email) values (26, 'Reeta', '2/9/1968', 'rferraronep@icio.us');
insert into employee (id, name, birthday, email) values (27, 'Ron', '9/3/1970', null);
insert into employee (id, name, birthday, email) values (28, 'Domini', '3/7/1994', null);
insert into employee (id, name, birthday, email) values (29, 'Malinde', '12/8/1995', 'mventhams@si.edu');
insert into employee (id, name, birthday, email) values (30, 'Malynda', '7/14/1974', null);
insert into employee (id, name, birthday, email) values (31, 'Stevana', '7/15/1968', 'skidwellu@quantcast.com');
insert into employee (id, name, birthday, email) values (32, 'Rey', '5/17/1978', 'rionsv@gmpg.org');
insert into employee (id, name, birthday, email) values (33, 'Yardley', '6/14/1982', null);
insert into employee (id, name, birthday, email) values (34, 'Darrin', '11/2/1979', 'dtunkinx@angelfire.com');
insert into employee (id, name, birthday, email) values (35, 'Reinold', '7/5/1995', 'rknightlyy@meetup.com');
insert into employee (id, name, birthday, email) values (36, 'Fonsie', '2/3/1979', null);
insert into employee (id, name, birthday, email) values (37, 'Emmye', '9/16/1972', null);
insert into employee (id, name, birthday, email) values (38, 'Hastie', '10/10/1998', null);
insert into employee (id, name, birthday, email) values (39, 'Ursula', '7/27/1989', 'uarni12@narod.ru');
insert into employee (id, name, birthday, email) values (40, 'Natale', '12/16/1977', 'ndevin13@pagesperso-orange.fr');
insert into employee (id, name, birthday, email) values (41, 'Clare', '11/4/1996', 'cfanton14@list-manage.com');
insert into employee (id, name, birthday, email) values (42, 'Shirlene', '8/28/1974', null);
insert into employee (id, name, birthday, email) values (43, 'Earl', '2/10/1971', 'ebartke16@twitpic.com');
insert into employee (id, name, birthday, email) values (44, 'Yettie', '6/6/1976', 'ywhaites17@oakley.com');
insert into employee (id, name, birthday, email) values (45, 'Cheryl', '2/19/1972', null);
insert into employee (id, name, birthday, email) values (46, 'Dela', '7/4/2009', 'dbrandsen19@typepad.com');
insert into employee (id, name, birthday, email) values (47, 'Vincent', '4/30/1970', null);
insert into employee (id, name, birthday, email) values (48, 'Fonsie', '8/25/1982', 'fmaxfield1b@fda.gov');
insert into employee (id, name, birthday, email) values (49, 'Oneida', '8/12/1995', 'oconradsen1c@4shared.com');
insert into employee (id, name, birthday, email) values (50, 'Orel', '3/1/1999', 'openhaleurack1d@cocolog-nifty.com');
```
3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```
UPDATE employee
SET name = 'Charm',
birthday = '1987-05-01',
email = 'charm@gmail.com'
WHERE id = 1;

UPDATE employee
SET name = 'jackie chan',
birthday = '1955-01-01',
email = 'jackiechan@hotmail.com'
WHERE id = 2;

UPDATE employee
SET name = 'angelina',
birthday = '1980-01-01',
email = 'angelinan@hotmail.com'
WHERE id = 30;

UPDATE employee
SET name = 'sparrow',
birthday = '1945-01-01',
email = 'jacksparrow@hotmail.com'
WHERE id = 12;

UPDATE employee
SET name = 'van dame',
birthday = '1945-01-01',
email = 'vandame@hotmail.com'
WHERE id = 25;
```
4. Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```
DELETE FROM employee
WHERE id = 3;

DELETE FROM employee
WHERE email = 'vandame@hotmail.com';

DELETE FROM employee
WHERE name LIKE 'La%';

DELETE FROM employee
WHERE name LIKE 'La%';

DELETE FROM employee
WHERE name LIKE 'La%';
```

My Patika account [Patika](https://academy.patika.dev/profile)

My Linkedin account [Linkedin](https://www.linkedin.com/in/cihangr/)

My GitHub account [GitHub](https://github.com/cihangr)