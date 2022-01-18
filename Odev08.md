# Odev 8

#### Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
~~~sql
 CREATE TABLE employee (
  id SERIAL PRIMARY KEY,
  name VARCHAR(50) NOT NULL,
  email VARCHAR(100),
  birthday DATE
);
~~~

#### Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
~~~sql
insert into employee (id, name, email, birthday) values (1, 'Adelle', 'aneve0@ibm.com', '05.07.1992');
insert into employee (id, name, email, birthday) values (2, 'Samuele', 'scolleer1@time.com', '10.08.1999');
insert into employee (id, name, email, birthday) values (3, 'Junia', 'jbezemer2@oracle.com', '23.12.1995');
insert into employee (id, name, email, birthday) values (4, 'Freddy', 'fbavage3@linkedin.com', '15.09.1994');
insert into employee (id, name, email, birthday) values (5, 'Amber', 'aturford4@a8.net', '05.01.1990');
insert into employee (id, name, email, birthday) values (6, 'Ramon', 'rrubinowitch5@people.com.cn', '10.07.1995');
insert into employee (id, name, email, birthday) values (7, 'Faye', 'frandal6@miitbeian.gov.cn', '14.09.1990');
insert into employee (id, name, email, birthday) values (8, 'Evonne', 'ebrasseur7@bloomberg.com', '14.06.1993');
insert into employee (id, name, email, birthday) values (9, 'Gwenneth', 'gfollin8@sbwire.com', '20.06.1990');
insert into employee (id, name, email, birthday) values (10, 'Riva', 'rnapolione9@ovh.net', '22.02.1990');
insert into employee (id, name, email, birthday) values (11, 'Cosimo', 'cchama@buzzfeed.com', '25.11.1992');
insert into employee (id, name, email, birthday) values (12, 'Olly', 'ococktonb@gov.uk', '20.07.1993');
insert into employee (id, name, email, birthday) values (13, 'Guthrey', 'gclappertonc@senate.gov', '09.06.1997');
insert into employee (id, name, email, birthday) values (14, 'Nadine', 'ncrossd@arizona.edu', '29.05.1996');
insert into employee (id, name, email, birthday) values (15, 'Harland', 'hworville@google.fr', '18.03.1994');
insert into employee (id, name, email, birthday) values (16, 'Alison', 'ahassardf@soundcloud.com', '01.10.1997');
insert into employee (id, name, email, birthday) values (17, 'Darci', 'dmccarlg@smugmug.com', '07.01.1998');
insert into employee (id, name, email, birthday) values (18, 'Shawn', 'stroughtonh@paginegialle.it', '17.05.1992');
insert into employee (id, name, email, birthday) values (19, 'Gussy', 'ggureryi@reuters.com', '28.07.1992');
insert into employee (id, name, email, birthday) values (20, 'Coralie', 'cwitheropj@nasa.gov', '13.09.1999');
insert into employee (id, name, email, birthday) values (21, 'Odelinda', 'obouldsk@eventbrite.com', '30.08.1990');
insert into employee (id, name, email, birthday) values (22, 'Wilie', 'wseamonl@pcworld.com', '10.04.1991');
insert into employee (id, name, email, birthday) values (23, 'Cassi', 'cmcneishm@digg.com', '03.08.1991');
insert into employee (id, name, email, birthday) values (24, 'Iggie', 'iphilipsn@prlog.org', '15.02.1993');
insert into employee (id, name, email, birthday) values (25, 'Sindee', 'ssymsono@phoca.cz', '17.12.1997');
insert into employee (id, name, email, birthday) values (26, 'Morey', 'mbolamp@yellowbook.com', '17.03.1992');
insert into employee (id, name, email, birthday) values (27, 'Hernando', 'hdreweryq@comcast.net', '08.08.1995');
insert into employee (id, name, email, birthday) values (28, 'Park', 'pwhetsonr@google.fr', '25.05.1993');
insert into employee (id, name, email, birthday) values (29, 'Brett', 'bmarners@usnews.com', '24.03.1997');
insert into employee (id, name, email, birthday) values (30, 'Kariotta', 'khryncewiczt@odnoklassniki.ru', '10.11.1993');
insert into employee (id, name, email, birthday) values (31, 'Gamaliel', 'gstaceu@thetimes.co.uk', '11.05.1995');
insert into employee (id, name, email, birthday) values (32, 'Coriss', 'cweakleyv@cafepress.com', '24.09.1998');
insert into employee (id, name, email, birthday) values (33, 'Karlens', 'klorinezw@ning.com', '03.10.1995');
insert into employee (id, name, email, birthday) values (34, 'Aldis', 'aginnix@ibm.com', '10.01.1998');
insert into employee (id, name, email, birthday) values (35, 'Hadria', 'helliotty@netvibes.com', '25.12.1995');
insert into employee (id, name, email, birthday) values (36, 'Adena', 'alauz@networksolutions.com', '02.06.1993');
insert into employee (id, name, email, birthday) values (37, 'Jordanna', 'jbland10@dropbox.com', '27.07.1994');
insert into employee (id, name, email, birthday) values (38, 'Veronique', 'vblei11@pbs.org', '16.10.1997');
insert into employee (id, name, email, birthday) values (39, 'Gloriana', 'gcostall12@uiuc.edu', '19.06.1999');
insert into employee (id, name, email, birthday) values (40, 'Lemmie', 'lchatell13@latimes.com', '16.02.1994');
insert into employee (id, name, email, birthday) values (41, 'Rodrique', 'rwickins14@nydailynews.com', '23.07.1996');
insert into employee (id, name, email, birthday) values (42, 'Antone', 'alathy15@purevolume.com', '13.10.1996');
insert into employee (id, name, email, birthday) values (43, 'Temple', 'tblyden16@tinyurl.com', '10.02.1995');
insert into employee (id, name, email, birthday) values (44, 'Melosa', 'mproudlock17@cisco.com', '27.11.1991');
insert into employee (id, name, email, birthday) values (45, 'Concordia', 'crubinowitz18@is.gd', '02.06.1997');
insert into employee (id, name, email, birthday) values (46, 'Hadley', 'hfrobisher19@hubpages.com', '14.04.1998');
insert into employee (id, name, email, birthday) values (47, 'Ali', 'atather1a@rambler.ru', '09.08.1990');
insert into employee (id, name, email, birthday) values (48, 'Ernie', 'ecasseldine1b@google.com.br', '05.12.1991');
insert into employee (id, name, email, birthday) values (49, 'Lissi', 'lringsell1c@fda.gov', '30.03.1991');
insert into employee (id, name, email, birthday) values (50, 'Agnella', 'ajohnsson1d@webmd.com', '05.06.1998');
~~~

#### Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
~~~sql
UPDATE Employee SET name = 'Ernique', birthday = '16.02.1994' WHERE id = 3;
UPDATE Employee SET birthday = '01.01.1998',name = 'Revaha' WHERE email = 'cmcneishm@digg.com';
UPDATE Employee SET birthday = '01.01.1991' WHERE email = 'hfrobisher19@hubpages.com';
UPDATE Employee SET name = 'Tom' WHERE id = 10;
UPDATE Employee SET email = 'templatemail@patikaodev.com' WHERE name = 'Sindee';
~~~

#### Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
~~~sql
DELETE FROM Employee WHERE email = 'templatemail@patikaodev.com';
DELETE FROM Employee WHERE id = '3';
DELETE FROM Employee WHERE name = 'Ernique';
DELETE FROM Employee WHERE name = 'Tom';
DELETE FROM Employee WHERE birthday = '01.01.1991';
~~~
