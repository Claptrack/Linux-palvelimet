## Komentokehotteen perusteet

Lukiessani Tero Karvisen artikkelia vuodelta 2020 (https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited) vahvistui aiempi näkemnykseni siitä, että Linuxin pyörittämisessä pärjää muutamalla tutulla komennolla, jotka tosiaan kannattaa opetella ulkoa. 

1. Jokaisella komennolla pitäisi olla oma man-sivu (esim. man df) joka esittää kyseisen komennon ohjesivun lessissä, tarkoittaen, että manuaali näyetään yhden sivun mittaisissa pätkissä ja sitä voi selata lessistä tutuilla näppäimillä (esim. space = seuraava, 'b' = edellinen, 'q' = quit).
2. SSH:lla voidaan turvallisesti ottaa etäyhteys toiseen työasemaan komentokehotteen kautta. Tämä mahdollistaa esim. samassa verkossa pyörivän linuxin hallitsemisen vaikka työkoneella pyörivän windowsin kautta.
3. Packet management (apt) mahdollistaa sovellusten asentamisen nopeasti ja turvallisesti. Ensimmäisenä tehdään 'sudo apt-get update', joka päivittää listan olemassa olevista paketeista. Tämän jälkeen paketteja voi asentaa 'sudo apt-get install' -komennolla. Pakettien asentaminen vaatii aina sudon käyttämistä, jolloin komentokehote kysyy "admin"-salasanaa.

Artikkelissa mainittujen komentojen lisäksi mainitsisin komennon 'df', joka näyttää työaseman eri tallennusmediat ja niiden kapasitetit sekä käytettävissä olevan tilan. Lisäämällä komentoon -h, lista näytetään "human-readable"-formaatissa.
