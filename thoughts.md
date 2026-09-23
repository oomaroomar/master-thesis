## RQ

Kuinka luotettavasti Cortex Analyst muodostaa käyttäjän tiedontarvetta vastaavia SQL-kyselyitä valitussa puhelinkeskusaineistossa, ja miten kysymysten toistaminen ja merkityksen säilyttävä uudelleenmuotoilu vaikuttavat kyselyiden semanttiseen vastaavuuteen ja keskinäiseen johdonmukaisuuteen?

## Maybe start johdanto with

Luonnollisen kielen muuntaminen SQL-kyselyiksi eli Text-to-SQL pyrkii mahdollistamaan tietokantojen hyödyntämisen ilman, että käyttäjän tarvitsee itse kirjoittaa SQL-kyselyitä. Kielimallipohjaisen järjestelmän hyödyllisyys riippuu kuitenkin siitä, vastaako tuotettu kysely käyttäjän tiedontarvetta. Syntaktisesti kelvollinen SQL-kysely voi esimerkiksi kohdistua väärään tietokantakenttään tai sisältää tarkoitukseen nähden virheellisen rajauksen tai aggregoinnin. Lisäksi järjestelmä voi tuottaa erilaisia kyselyitä saman kysymyksen toistoissa tai silloin, kun kysymyksen sanamuotoa muutetaan sen merkitystä muuttamatta.

Tässä tutkielmassa tarkastellaan, kuinka luotettavasti Snowflaken Cortex Analyst muodostaa käyttäjän tiedontarvetta vastaavia SQL-kyselyitä valitussa puhelinkeskusaineistossa ja miten kysymysten toistaminen ja merkityksen säilyttävä uudelleenmuotoilu vaikuttavat kyselyiden semanttiseen vastaavuuteen ja keskinäiseen johdonmukaisuuteen. Tutkimuksessa erotetaan SQL-kyselyiden muodollinen vaihtelu niiden merkitystä muuttavista eroista. Tavoitteena on arvioida paitsi tuotettujen kyselyiden vastaavuutta tiedontarpeeseen myös sitä, millaisissa tilanteissa vastaavuus ei säily.

## Contribution

Tutkielman kontribuutio Text-to-SQL-tutkimukseen on rajattu tapaustutkimus semanttista näkymää hyödyntävän kaupallisen järjestelmän SQL-tuotosten semanttisesta vastaavuudesta ja johdonmukaisuudesta. Analyysissa erotetaan kyselyiden muodollinen vaihtelu tiedontarpeen toteutumiseen vaikuttavista eroista sekä tarkastellaan kysymysten toistamisen ja merkityksen säilyttävän uudelleenmuotoilun yhteydessä ilmeneviä virhetyyppejä. Tutkimus tuottaa tapauskohtaista tietoa järjestelmän toiminnasta, mutta ei pyri arvioimaan sen yleistä suorituskykyä kaikissa Text-to-SQL-tehtävissä.
