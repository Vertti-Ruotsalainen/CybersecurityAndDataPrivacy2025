## Portswigger
>
> <img width="1760" height="629" alt="kuva" src="https://github.com/user-attachments/assets/d509a896-db9c-48ff-bca6-cd47a0b018da" />


* SQL injection vulnerability in WHERE clause allowing retrieval of hidden data
* SQL injection vulnerability allowing login bypass
* File path traversal, simple case
* Unprotected admin functionality
* Unprotected admin functionality with unpredictable URL
* User role controlled by request parameter
* User role can be modified in user profile
* User ID controlled by request parameter
* User ID controlled by request parameter, with unpredictable user IDs
* User ID controlled by request parameter with data leakage in redirect
* User ID controlled by request parameter with password disclosure
* Insecure direct object references
* Username enumeration via different responses
* 2FA simple bypass
* Password reset broken logic
* SQL injection UNION attack, determining the number of columns returned by the query


## Booking system project

Phase 1:

Projektin alussa ladattiin joko työpöytä tai virtuaalikoneesseen testiympäristö (Docker, Zap, etc)
* Alkuun jouduin ongelmiin valittuani virtuaalikone lähestymistavan projektin alussa. Tämä johtui unohdetuista opeista ja komennoista liittyen linux pohjaiseen toimintatapaan.
* Kaiken conffauksen jälkeen ajettiin ZAP hyökkäykset ja etsittiin haavoittuvuuksia rekisteröinti sivulta.
* Phase 1 part 2 tehtiin samat ZAP hyökkäykset ja todettiin että haavoittuvuuksia ei näkyny enää (Ainakaan ZAP mukaan)

Phase 2:

* Harjoiteltiin salasanojen crackkamista offlinessa.
* Tämän taskin aikana opin etsimään/käyttämään tunnettuja salasanalistoja ja tutustuin bruteforcessa käytettäviin ohjelmiin.
* Eniten aikaa vievää oli odottaa kun ajat 10000000000 vaihtoehdosta salasana bruteforcen testimielessä.

Phase 3:

Teemana oli:
    Authorization
    Logging
    Security testing
    Shielding
    GDPR

* Tehtiiin Authorization Testing Assignment, jossa katsottiin mitä/mihin/milloin/koska/kun käyttäjä  tyypeillä on pääsy (Quest, reserver, admin)
* Osiossa oli parasta miettiä millä kaikilla tekniikoilla pystyi rikkomaan koko "tietoturvan" ja tämä vei samalla eniten aikaa kun kokeilin manuaalisesti eri komentoja.
* Samalla tutustuttin gobusterin käyttöön joka oli melko sekavaa alussa ja en mielestäni sisäistänyt kaikkia mahdollisuuksia tätä käytettäessä.

Phase 4:

    GDPR compliance testing
    Adding Privacy Policy to the app

* Tässä osiossa keskityttiin enimmäkseen GDPR näkökulmasta sivustoon.
* Tehtiin GDPR check lista.
* Kirjoitettiin sivulle haluamansa cookieprivacy, termofservice ja pricypolicyt


Tiivistelmä 

Tässä projektissa opin paljon käytännön asioita kyberturvallisuudesta ja tietosuojasta. Alussa työkalujen
käyttöönotto oli haastavaa, mutta samalla opin käyttämään niitä paremmin, kuten ZAPia haavoittuvuuksien
etsimiseen. Salasanojen crackkaus auttoi ymmärtämään, miksi vahvat salasanat ovat tärkeitä.
Authorization-testauksessa huomasin, miten helposti käyttöoikeuksia voi yrittää kiertää. GDPR-osiossa
opin, mitä asioita sivustolla pitää huomioida käyttäjän yksityisyyden ja lakivaatimusten kannalta.

## Logbook

https://github.com/Vertti-Ruotsalainen/CybersecurityAndDataPrivacy2025/blob/main/logbook.md

* 74,5 hours total used
* Phase1 : ~22h
* Phase2 : 6-7h
* Phase3 : 6h
* Phase4 : 6h
* So about 40h~ hours for project and 34h for labs, reading material, searching info, testing and doing cisco tasks.


## Feedback

* Kurssi oli kaiken puolin tosi opettavainen. Tyyli jolla kurssia käytiin oli mahtava, käytännön tekeminen on omastamielestäni paras tapa oppia uusia ja kerrata vanhoja oppeja.
* Toki kurssin aikana tuli huomattua, ettei ole vielä löytyny sitä kultaista keskitietä kurssisisällölle. Kurssia kun on vai pidetty muutaman kerran.
* Kokonaisuutena kurssi oli siis mahtava. Jatka samaan malliin niin tästä rakentuu vielä mahtava oppikokonaisuus tulevaisuuden opiskelijoille.









