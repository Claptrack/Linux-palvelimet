## Rauta

Tällä komennolla 'sudo lshw -short -sanitize' hain tietoa koneeni hardwaresta, ja sain tuloksena helppolukuisen listan koneen komponenteista ja niiden poluista

<img width="1116" alt="image" src="https://github.com/user-attachments/assets/ba92aeed-2094-4a5a-bb71-2deec69609c6">

Ensimmäisenä kerrotaan tiedot järjestelmästä, joka tässä tapauksessa on Raspberry PI 4 B

/0 kuvaa järjestelmän emolevyä

/0/1 alkaen kuvataan prosessoria: Prosessorilla on neljä ydintä joilla kaikilla on 32 kilotavua välimuistia

/0/6 kuvaa järjestelmän RAM-muistia, joka tässä tapauksessa on pyöristettynä 4 gigatavua

/0/0 kuvaa PCIe-siltaa, johon kaikki tämän alla olevat laitteet ovat liitetty

/0/0/0/0 ja /0/0/0/1 kuvaa USB-liitintä 1 ja 2, ja niiden alla on kuvattu laitteet, jotka kyseisiin liitäntöihin on yhdistetty. Tässä järjestelmässä ei ole sisäänrakennettua kovalevyä (Raspeissa se on vakiona SD-kortti, joka ei kestä kauhean hyvin esim. sähkökatkoja), vaan käyttöjärjestelmä on ulkoisella SSD-levyllä /dev/sda

/1 ja /2 kuvaa järjestelmän verkkoliitännät. Tässä laitteessa on sekä ethernet- että wlan-liitännät.

## Lähteet

Tehtävänanto: https://terokarvinen.com/linux-palvelimet/#h2-komentaja-pingviini


