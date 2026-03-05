# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Hajautettu Git -osuus aiheutti minulle ehdottomasti eniten haasteita. GitHubin käyttö on minulle jokseenkin entuudestaan tuttua, joten etärepositorion luominen ja yhdistäminen sujuivat hyvin. Kurssimateriaali antoi hyvät eväät suorittaa tehtävää ja erilaisia komentoja selityksineen oli riittävästi tarjolla. 

Kohtasin kuitenkin ongelmia kun yritin puskea paikallisen repositorioni Githubiin. Oletin, että pääsisin kirjautumaan terminaalissa käyttäjälleni GitHubiin mutta törmäsin virheilmoitukseen:

        remote: Invalid username or token. Password authentication is not supported for Git operations.
        fatal: Authentication failed for 'https://github.com/sauna41/Git_versionhallinta.git/' 
        

Lähdin selvittämään asiaa ja kävi ilmi, että GitHub ei enää salli salasanan käyttöä git push tai pull-komentohin HTTPS:n kautta. Jouduin luomaan Personal Access Tokenin (PAT) GitHubin Developer Settingseistä, jolle määritin read & write -oikeudet Contents, Pull Requests, Actions & Workflow osuuksiin. Tokenin avulla sain lopulta puskettua main-haaran Githubiin. 

Token selvitelyä lukuunottamatta harjoitus sujui hyvin. Paikallisen ja etärepositorion suhde tuntui helposti ymmärrettävältä mutta committien "jälkeenjääminen", kuten *“Your branch is behind ‘origin/main’ by 1 commit”* vaati hieman ajatustyötä ennen kuin ymmärsin miten muutokset liikkuvat repositorioiden välillä. 


## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| git remote add origin "etärepositorion URL| lisää etärepositorion paikalliseen Gittiin |
| git remote -v | näyttää liitetyt etärepositoriot |
| git push -u origin main | lähettää paikallisen haaran etärepositorioon |
| git fetch | noutaa uusimmat muutokset etärepositoriosta |
| git checkout origin/main | vaihtaa paikallisesti haaraa etärepositorion main-haaraan |
| git checkout main | vaihtaa työtilan main-haaraan |
| git merge origin/main | yhdistää etärepositorion main-haaran muutokset paikaliseen haaraan |

+ näiden lisäksi paljon samoja komentoja, kuin aiemmissa harjoituksissa. Lisää komentoja on listattuna [oppimispaivakirja2](paivakirja1.md) 
