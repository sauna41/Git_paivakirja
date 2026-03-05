# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Olen aikoinaan harjoitellut Gitin peruskäyttöä, joten minulta löytyi valmiiksi vaadittava ympäristö (*Git, Visual Studio Code & GitHub*).

Paikallisen Gitin harjoitukset 1-4 olivat hyvin samanlaisia, mitä olen joskus aiemmin suorittanut, joten ne eivät tuottaneet juurikaan ongelmia. Master- ja main-haarojen eroja jouduin hieman selvittelemään, sillä olen aiemmin oppinut main -termin, mikä ilmeisesti on nykyään masteria yleisemmin käytössä oleva termi. 

Haarojen vaihtaminen ja niiden mergeäminen vaati hieman pohdintaa. Asia selkeni hyvin, kun lopulta suoritin *git merge --no-ff* -komennon ja tarkastelin lokia, missä haarojen yhdistyminen oli mielestäni esitetty suht selkeästi.  

index.html:än muokkaaminen ja tutkiminen sekä main- että tyylit-haarassa oli mielestäni loistava tapa havainnollistaa miten eri haarat toimivat. Helpotti ymmärtämään, miten muutoksia voidaan luoda eri haaroissa sotkematta koko projektia. 

*git restore / revert* olivat myös itselleni uusia asioita. Ne vaativat hieman kurssimateriaaleihin perehtymistä ja erityisesti revert oli itselleni syystä tai toisesta monimutkainen asia. Luin kuitenkin kurssimateriaalin useaan otteeseen ja tutkin myös muita lähteitä näiden komentojen osalta.  

Tehtävät ehdottomasti virkistivät muistiani Gitin peruskomentojen osalta. git add & git commit muistuivat hyvin mieleen ja tiedostojen lisääminen/poistaminen repositoriosta tuntui loogiselta.  

Ehdottomasti eniten kertaamisen tarvetta syntyi Git lokin tulkitsemisessa ja hyödyntämisessä. Loki tuntui antavan niin paljon informaatiota, että etsityn tiedon löytäminen tekstiseinästä oli haastavaa. 

## Osiossa käyttämäni Git-komennot


| git init | luo uuden Git-repositorion nykyiseen hakemistoon |

| git status | näyttää git työtilan tilan |

| echo | tulostaa tekstiä / kirjoittaa tiedostoon |

| git add | lisää muutokset Gitin valmistelualueelle ennen tallennusta |

| git commit -m | tallentaa valmistelualueella olevat muutokset repositoriohistoriaan ja jättää commit-viestin |

| git status | näyttää repositorion sen hetkisen tilanteen |

| git mv | siirtää tai uudelleennimeää tiedoston |

| git rm | poistaa tiedoston |

| git log | näyttää commit historian |

| git log -stat | näyttää commit historian sekä tiedostomuutokset |

| git tag | luo merkinnän tuoreimpaan commit versioon |

| git restore | palauttaa tiedoston aikaisempaan versioon / peruuttaa tehdyt muutokset |

| git revert | kumoaa aiemman commitin uudella commitilla |

| git branch "haaranNimi" | luo uuden haaran (branch) |

| git checkout "haaranNimi"| vaihtaa haaraa |

| git merge --no-ff | yhdistää haaran toiseen haaraan pakottamalla merge-commitin |

+ näiden lisäksi komentorivin yleisiä cd, mv, yms komentoja, joita en listannut "git" -komennoiksi. 



