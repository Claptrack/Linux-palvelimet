# Linuxin asentaminen virtuaalikoneelle

Tässä raportissa käyn läpi askel askeleelta sen, miten asensin Linuxin virtuaalikoneelle. Päätin käyttää hyväkseni Teemu Laineen ohjetta: https://github.com/HortTemppa/horttemppa.github.io/blob/main/h1.md, koska taloudessamme on tällä hetkellä käytössä ainoastaan M1 Mac (käyttiksenä Sequioa 15.0 Beta).

## Virtualisointiohjelmiston lataaminen

1. Ensin latasin UTM:n asennuspaketin ja asensin sen (https://mac.getutm.app/). Lataus ja asennus hoitui parissa minuutissa.

    <img width="1172" alt="image" src="https://github.com/user-attachments/assets/73692adc-a526-4fe0-858b-a70ed1c696df">

## Linux ISOn lataaminen UTM:ään

1. Asennuksen jälkeen avasin UTM:n ja klikkasin "Browse UTM gallery"

    <img width="409" alt="image" src="https://github.com/user-attachments/assets/f82573e7-de5a-49ce-a0bc-be9a5a843d71">

2. Valitsin listalta Debian 11 (LXDE) ja klikkasin "Open in UTM". Tämä aloitti Debian 11 ISOn lataamisen UTM:ään.

   <img width="772" alt="image" src="https://github.com/user-attachments/assets/19b25ed3-280d-4b22-b3b3-6fd13255dbf5">

## Virtuaalikoneen konfigurointi ja käyttiksen lataaminen

1. Ennen käyttöjärjestelmän lataamista avasin virtuaalikoneen asetukset klikkaamalla valikosta Edit

    <img width="926" alt="image" src="https://github.com/user-attachments/assets/c70e2174-1d9b-4174-bfdf-d575a059b90e">

2. Information-välilehdellä vaihdoin kirjautumiseen käytettävän salasanan, sekä root-salasanan

    <img width="808" alt="image" src="https://github.com/user-attachments/assets/f1eb7bd6-a848-4c16-af3a-119a67841e1e">

3. System-välilehdellä muutin virtuaalikoneen käytettävissä olevan RAM-muistin 4:ään gigatavuun.

    <img width="801" alt="image" src="https://github.com/user-attachments/assets/12e1093d-1867-4ee8-adec-2b49edfad99c">

4. Tämän jälkeen tallensin asetukset ja klikkasin käyttiksen kuvaa käynnistääkseni sen. Hetken päästä olin jo kirjautumisikkunassa.

   HOX! Kirjautumisessa en päässyt sisään käyttäjätunnuksella ja salasanalla, jotka olin aiemmin tallentanut. Jouduin siis kirjautumaan käyttämällä defaultia (debian/debian).

    <img width="701" alt="image" src="https://github.com/user-attachments/assets/c06c3fec-1708-4dff-a1fa-351f37b0b184">

6. Sisäänkirjautumisen jälkeen kokeilin ensimmäisenä, että pääsen internetiin. Selain ei kuitenkaan auennut, vaan palautti seuraavan virheilmoituksen:

    <img width="430" alt="image" src="https://github.com/user-attachments/assets/853d1789-2ed9-420d-9d25-4ea9829aa8e3">

7. Etsin virheilmoituksella tietoa netistä ja löysin tämän tuloksen, jossa kehotettiin tarkistamaan käyttiksen "default" selain: https://unix.stackexchange.com/questions/403836/error-invalid-desktop-entry-file-when-using-web-browser-in-lxde. Asetuksissa selvisi, että selainta ei jostain syystä ole lainkaan tässä käyttöjärjestelmässä.
    
8. Menin asetuksiin täältä:

    <img width="453" alt="image" src="https://github.com/user-attachments/assets/dfa02368-5fad-4167-a046-1cb39939e360">
    
    <img width="729" alt="image" src="https://github.com/user-attachments/assets/71d290b2-7094-4644-8f5c-bfd3618f1804">

9. Kokeilin myös käynnistää selaimen komentokehotteen kautta

    <img width="658" alt="image" src="https://github.com/user-attachments/assets/0a3e1150-47bb-49f2-a484-c69356f84668">

10. Jos aikaa olisi enemmän, lataisin toisen distron UTM:ään ja kokeilisin uudestaan.
    

    
