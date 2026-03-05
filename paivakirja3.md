# Oppimispäiväkirja: Git projektissa

__Mitä hyötyä voisi olla versionhallinnasta, jos kehität projektia yksin?__

Versionhallinta helpottaa projektin edistymisen seuraamista. Lokit kertovat, mitä milloinkin on tehty ja tarvittaessa voidaan palata tiettyyn aiempaan kohtaan projektia. Versionhallinnan avulla voidaan myös kehittää projektin eri haaroja erillisinä toisistaan ilman, että koko projekti sotkeutuu esimerkiksi virheen johdosta. 

Projekti on myös mahdollista varmuuskopioida tai siirtää toiselle käyttäjälle tai koneelle.

__Mitä hyötyä voisi olla versionhallinnasta, jos projektissa on useita kehittäjiä?__

Jos projektissa työskentelee useampi kehittäjänä, versionhallinnan avulla jokaisen on mahdollista työskennellä projektin parissa samanaikaisesti. Eri jäsenet voivat kehittää projektia eri haaroissa ilman, että tiimiläiset kirjoittavat toistensa päälle. Jos konflikteja, eli muutosten yhteentörmäyksiä, versionhallinta auttaa havaitsemaan ja korjaamaan ne. Lopuksi kaikki yhdistetään hallitusti toimivaksi kokonaisuudeksi. 

Versionhallinta jättää myös lokiin dokumentaatiota siitä, mitä muutoksia kukakin on milloinkin tehnyt. Projekti on myös mahdollista varmuuskopioida ja tarvittaessa palauttaa. 


__Miten järjestäisit projektitiimin versionhallinnan 3-4 hengen ohjelmistoprojektikurssilla? Laadi tiimiläisille lyhyt ohje, miten projektissa toimitaan.__

1. Haarat:
    - Käytetään main-päähaaraa vain valmiille ja testatuille muutoksille
    - Jokaisella ominaisuudelle oma feature-haaransa, jotka yhdistetään main-haaraan kun ominaisuus on saatu valmiiksi
2. Commitit: 
    - Tee pieniä ja selkeitä committeja useasti.
        - Tee commit vain yhdestä ominaisuudesta, ei kokonaisuudesta kerrallaan
    - Jätä committeihin kuvaava viesti siitä, mitä on tehty. Esimerkiksi "Lisätty kellopainikkeen js-skripti."
3. Push ja Pull:
    - Työskentele aina uusimpien muutosten kanssa. Käytä git fetch / git pull ennen uuden commitin puskemista.
    - Puske omat committisi etärepositorioon säännöllisesti
4. Merge
    - Kun tietty osuus on valmis, yhdistä se main-haaraan git merge -komennolla
    - Hyödynnä tarvittaessa Pull Requestia
5. Konfliktien hallinta
    - Jos kohtaat merge conflicteja, pyri ratkaisemaan ne välittömästi ja dokumentoi, mitä konfliktista jäi voimaan ja mitä poistettiin. 
6. Dokumentaatio
    - Kerää dokumentaatio toiminnastasi koko projektin ajan:
        - käytetyt komennot
        -  virheilmoitukset ja niiden ratkaisut
        - uudet toiminnallisuudet
7. Tiimin yhtenäiset käytännöt
    - Säännöllinen kommunikointi projektin etenemisestä ja vaiheista
    - Yhdistä main-haaraan vain toimivia ominaisuuksia
    - Käytä tägejä, kuten v.1.0 pitkin projektia
    - Kunnioita tiimin yhdessä sovittuja toimintatapoja


__Kommenttini opintojaksosta, esim. sisällöstä, materiaalista, työmäärästä, hyödyllisyydestä, työmäärästä. Mitä toivoisit olevan enemmän, mitä vähemmän?__

Kurssin hyödyllisyys oli ehdottomasti merkittävin tekijä, miksi halusin suorittaa kurssin mahdollisimman nopeasti. Oman kokemukseni ja kuulemani mukaan, Git versionhallinta on todella laajalla käytöllä ja siten tärkeä työkalu usealla osa-alueella niin kouluprojekteissa kuin tulevaisuuden työelämässä. Koin, että kurssi antoi hyvät eväät Git-versionhallinnan alkeisiin, joilla pystyisi jo hyvin toteuttamaan esimerkiksi ohjelmointiprojektin.

Kurssimateriaali oli hyvää ja sitä oli mielestäni helppo seurata. Olin aiemmin oppinut puhumaan päähaarasta main-haarana, kun taas materiaaleissa käytettiin master-haaraa. Tämä aiheutti itselleni alussaa hieman selvittelyä, kuinka ne eroavat toisistaan mutta jäin siihen käsitykseen, että main-haara on nykyään yleisemmin käytössä. 

Valtaosa harjoituksista eteni sulavasti ohjeen mukaan, mutta joissakin kohdissa, kuten Git projektissa -osuudessa jouduin selvittelemään asioita itsenäisesti kun en löytänyt kurssimateriaaleista vastausta. En ainakaan itse löytänyt materiaaleista myöskään tietoa siitä, että GitHub ei enää salli puskemisen ilman ssh-avainta tai tokenia, joten tämän selvittely aiheutti jonkin verran harmaita hiuksia.

Työmäärä tuntui mielestäni maltilliselta. Jotta toistoja saisi vielä hieman enemmän, voisi harjoituksissa olla vielä enemmänkin tavaraa. Esimerkiksi konfliktien ratkaisu jäi vielä hieman epäselväksi. 