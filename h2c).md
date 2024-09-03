## Tärkeät hakemistot Linuxissa

# '/', eli root

Järjestelmän ylin parent-kansio, joka sisältää kaikki muut hakemistot. Root on verrattavissa Windowsin C: -hakemistoon. Linuxissa ei käytetä kirjaimia.

<img width="808" alt="image" src="https://github.com/user-attachments/assets/c7431603-81ae-478e-a88b-33b0ede869dd">

# /home/, eli kotihakemisto

<img width="808" alt="image" src="https://github.com/user-attachments/assets/75ad3838-901d-4dcf-bec0-9aa0b78111cb">

Täältä löytää kaikkien käyttäjien omat hakemistot, jotka pitävätä sisällään käyttäjäkohtaiset kansiot työpöydälle, dokumenteille, kuville jne. Tällä työasemalla on ainoastaan yksi käyttäjä (claptrack).

<img width="808" alt="image" src="https://github.com/user-attachments/assets/3e023ab9-419f-4b85-b16e-c9b4e2024a94">

# /etc/ on hakemisto asetustiedostoille

Tästa hakemistosta löytyy järjestelmän tallennetut tekstimuotoiset asetustieodostot.

<img width="808" alt="image" src="https://github.com/user-attachments/assets/46cd2f1e-37bc-4ebe-bf56-d18bd1edaeba">

Esimerkkinä hakemisto 'ufw', joka sisältää asentamani palomuuriohjelmiston asetukset.

<img width="808" alt="image" src="https://github.com/user-attachments/assets/e1325b65-c52d-455a-936d-a549d6c2f61a">

Tiedosto ufw.conf pitää sisällään asetustiedoston, johon voi tarvittaessa tehdä muutoksia esim. ohjelman automaattiseen käynnistymiseen

<img width="808" alt="image" src="https://github.com/user-attachments/assets/d0e6cc5f-fef1-4a47-ab69-422d342d2c47">

# /media/ on hakemisto esim. ulkoisille kovalevyille tai cd-asemille

<img width="808" alt="image" src="https://github.com/user-attachments/assets/6f949754-f4c4-429e-ba40-5813b637c5dd">

Minun tapauksessani yhdistetyt kovalevyt eivät näy ja epäilen syyksi sitä, että ne ovat auto-mountattu (asetettu yhdistymään aina tiettyyn kansioon) toisen hakemiston kansioihin.

# /var/log/ -hakemistosta löytyy lokitiedostot, joita järjestelmä luo

<img width="808" alt="image" src="https://github.com/user-attachments/assets/2379c335-1ec7-4492-954e-5795b07bcfec">

Jotta pääsin lukemaan tiedostojen sisällön, piti käyttää sudoa, esim. 'sudo micro ufw.log'

Tässä tiedostossa on käsitykseni mukaan loki laitteista, jotka ovat yrittäneet ottaa yhteyttä Raspiini

<img width="808" alt="image" src="https://github.com/user-attachments/assets/4cca5ff9-aa48-4971-8845-690d3026339a">

## Lähteet

Tehtävänanto: https://terokarvinen.com/linux-palvelimet/#h2-komentaja-pingviini
Command Line Basics Revisited, Tero Karvinen 2020: https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited
