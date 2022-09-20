# SQL-8


- Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

`
CREATE TABLE employee
(
  id int,
  name VARCHAR(50),
  birthday DATE,
  email VARCHAR(100)
)
`

- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

`
insert into employee (id, first_name, birthday, email) values (1, 'Lettie', '1978-04-10', 'lsalmons0@soup.io');
insert into employee (id, first_name, birthday, email) values (2, 'Adel', '2004-10-24', 'abrodbin1@zimbio.com');
insert into employee (id, first_name, birthday, email) values (3, 'Lucille', '1976-05-18', 'lmacpeake2@sakura.ne.jp');
insert into employee (id, first_name, birthday, email) values (4, 'Pearl', '1994-12-22', 'pelverstone3@irs.gov');
insert into employee (id, first_name, birthday, email) values (5, 'Gallard', '1962-07-17', 'gagdahl4@tripod.com');
insert into employee (id, first_name, birthday, email) values (6, 'Davey', '2007-02-18', 'droget5@google.nl');
insert into employee (id, first_name, birthday, email) values (7, 'Cody', '2021-01-07', 'cundy6@wunderground.com');
insert into employee (id, first_name, birthday, email) values (8, 'Allistir', '1996-07-21', 'aaubry7@mapquest.com');
insert into employee (id, first_name, birthday, email) values (9, 'Bail', '2004-03-21', 'bmerriment8@dedecms.com');
insert into employee (id, first_name, birthday, email) values (10, 'Carlotta', '1952-10-30', 'cdeneve9@cbc.ca');
insert into employee (id, first_name, birthday, email) values (11, 'Cale', '2016-10-07', 'candrieua@clickbank.net');
insert into employee (id, first_name, birthday, email) values (12, 'Dodie', '2001-10-16', 'dsimoniteb@51.la');
insert into employee (id, first_name, birthday, email) values (13, 'Dennison', '1996-10-06', 'dtouhigc@harvard.edu');
insert into employee (id, first_name, birthday, email) values (14, 'Caren', '1961-01-11', 'cbungeyd@soundcloud.com');
insert into employee (id, first_name, birthday, email) values (15, 'Ike', '2010-09-13', 'ibabee@live.com');
insert into employee (id, first_name, birthday, email) values (16, 'Carmella', '2011-03-25', 'cscholardf@g.co');
insert into employee (id, first_name, birthday, email) values (17, 'Mack', '1973-04-22', 'mshelborneg@engadget.com');
insert into employee (id, first_name, birthday, email) values (18, 'Modestia', '2007-11-21', 'msothebyh@about.me');
insert into employee (id, first_name, birthday, email) values (19, 'Tiler', '1976-05-19', 'tcleaveri@yelp.com');
insert into employee (id, first_name, birthday, email) values (20, 'Morgen', '2006-05-27', 'mlidellj@a8.net');
insert into employee (id, first_name, birthday, email) values (21, 'Galven', '1969-09-09', 'gharridgek@flickr.com');
insert into employee (id, first_name, birthday, email) values (22, 'Benni', '2008-12-15', 'brichardinl@mozilla.org');
insert into employee (id, first_name, birthday, email) values (23, 'Vikky', '2010-08-27', 'vbonnetm@microsoft.com');
insert into employee (id, first_name, birthday, email) values (24, 'Farley', '1984-02-24', 'fsounessn@yahoo.com');
insert into employee (id, first_name, birthday, email) values (25, 'Ammamaria', '1971-12-16', 'adiviso@chicagotribune.com');
insert into employee (id, first_name, birthday, email) values (26, 'Jefferey', '1965-02-19', 'jspeachleyp@wiley.com');
insert into employee (id, first_name, birthday, email) values (27, 'Tierney', '2002-09-04', 'tdanilchenkoq@mlb.com');
insert into employee (id, first_name, birthday, email) values (28, 'Kassey', '1960-09-05', 'kswetmanr@google.co.uk');
insert into employee (id, first_name, birthday, email) values (29, 'Ivory', '2001-08-09', 'iviels@dailymail.co.uk');
insert into employee (id, first_name, birthday, email) values (30, 'Ashien', '1952-03-05', 'agibbinst@amazonaws.com');
insert into employee (id, first_name, birthday, email) values (31, 'Jackelyn', '1992-02-19', 'jcaldairouu@abc.net.au');
insert into employee (id, first_name, birthday, email) values (32, 'Vance', '1995-10-14', 'vmarsonv@elegantthemes.com');
insert into employee (id, first_name, birthday, email) values (33, 'Lolita', '2013-08-22', 'ldunckleew@slideshare.net');
insert into employee (id, first_name, birthday, email) values (34, 'Joanie', '1981-01-31', 'jslatfordx@opensource.org');
insert into employee (id, first_name, birthday, email) values (35, 'Micaela', '2014-08-06', 'mbenedity@weibo.com');
insert into employee (id, first_name, birthday, email) values (36, 'Aliza', '1989-07-20', 'apottz@ca.gov');
insert into employee (id, first_name, birthday, email) values (37, 'Ekaterina', '1959-02-16', 'etrahearn10@tumblr.com');
insert into employee (id, first_name, birthday, email) values (38, 'Ginevra', '1984-11-24', 'ghardwin11@nifty.com');
insert into employee (id, first_name, birthday, email) values (39, 'Fair', '2017-07-30', 'ffisbey12@blogger.com');
insert into employee (id, first_name, birthday, email) values (40, 'Merrill', '2009-12-10', 'mhannond13@ed.gov');
insert into employee (id, first_name, birthday, email) values (41, 'Lorraine', '2018-03-16', 'lhaskayne14@dailymotion.com');
insert into employee (id, first_name, birthday, email) values (42, 'Joanie', '1969-12-12', 'jhaacker15@theglobeandmail.com');
insert into employee (id, first_name, birthday, email) values (43, 'Diane', '2004-12-31', 'dcowpe16@mac.com');
insert into employee (id, first_name, birthday, email) values (44, 'Nikoletta', '1997-04-07', 'nhardeman17@seesaa.net');
insert into employee (id, first_name, birthday, email) values (45, 'Nixie', '2021-07-10', 'nstigers18@bloglines.com');
insert into employee (id, first_name, birthday, email) values (46, 'Kiley', '2001-03-16', 'kboncoeur19@drupal.org');
insert into employee (id, first_name, birthday, email) values (47, 'Jory', '1955-08-24', 'jmcneil1a@weather.com');
insert into employee (id, first_name, birthday, email) values (48, 'Wyn', '1973-05-06', 'wkelner1b@google.com.br');
insert into employee (id, first_name, birthday, email) values (49, 'Cyb', '2012-05-17', 'cschimonek1c@ow.ly');
insert into employee (id, first_name, birthday, email) values (50, 'Chaddy', '1971-02-06', 'cmckean1d@e-recht24.de');
`



- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

`
UPDATE employee
SET
  name = 'Maide'
WHERE id = 2

----------
UPDATE employee
SET
  name = 'Mei'
WHERE id = 13

----------

UPDATE employee
SET
  name = 'Ashley'
WHERE id = 17

----------
UPDATE employee
SET
  name = 'Commit'
WHERE id = 32
----------
UPDATE employee
SET
  name = 'Made'
WHERE id = 5

----------
`

- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

`
DELETE FROM employee
WHERE id = 34
`
---------
`
DELETE FROM employee
WHERE id = 4`
---------
`
DELETE FROM employee
WHERE id = 45`
---------
`
DELETE FROM employee
WHERE id = 14`
---------
`
DELETE FROM employee
WHERE id = 24
`
---------


