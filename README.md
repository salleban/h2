# h2
Linux terminal

# Termial

Aloitus käy mukavasti. Huomaan Virtuaalikonetta käynnistäessä saavani virheen, että tiedostot puuttuvat. Eli asentelen uudelleen VirtualBoxin..

Sitten itse aiheeseen. Lähdin rakentamaan hakemistoa touch menetelmällä. Mutta ensin avasin Terminalin ja katsastelin olemassa olevat hakemistot läpi. 

![Kuva 1](https://user-images.githubusercontent.com/100162043/213856476-d8308e8d-bf2e-4457-9778-a307bf8400a6.jpg)


Käytin pwd hakua selvittääkseni, missä hakemistossa olen ja tämän jälkeen selvitin ls hakua selvittääkseni mitä Home kansion alta löytyy. 

## Hakemisto

Hakemiston nimeäminen ja luominen tapahtuu mkdir komennon avulla. Kirjoittamalla mkdir ja perään haluamasi nimi hakemistolle, syntyy hakemistokansio. Esimerkiksi:

        $ mkdir Days 
        
Nähdäksesi onnistuiko hakemiston luominen kirjoita:

        $ ls
        
![Kuva 2](https://user-images.githubusercontent.com/100162043/213856559-f48e3413-12f7-49be-a02d-01b235879d50.jpg)


Näin huomaan luoneeni Days hakemiston muiden joukkoon. 

## Hakemiston alakansiot

Seuraavan vuorossa on lisätä Days hakemistoon kansioita. Tyhjennetään tässä vaiheessa terminaali painamalla ctrl + L. 
Katsoin kirjoittamalla pwd, että olenko varmasti Home kansiossa tyhjennettyäni terminaalin ja huomasin olevani edelleen uudella luomallani Days kansiossa. 

![Kuva 3](https://user-images.githubusercontent.com/100162043/213856614-8b5029f9-236b-4e57-ab58-178f7192f4c5.jpg)


Hakemiston saa ns. nollattua kirjoittamalla terminaaliin cd ~. Nyt kirjotan uudestaan pwd ja huomasin olevani takaisin home kansiossa. 

Seuraavaksi luokdaan Days hakemiston alle viikonpäivän hakemistot. Tämä tapahtuu kirjoittamalla: 

        $ mkdir -p Days/mon

Katsoammeksemme toimiko tämä komento, kirjoitetaan: 

        $ cd Days
        $ ls
        
Ja huomaan kuvan mukaisesti, että mon niminen hakemisto on luotu Days hakemiston alle. 

![Uusikuva 4](https://user-images.githubusercontent.com/100162043/213856694-ea206993-d4e7-450b-a6d6-524effdc0bb5.jpg)




        $ mkdir -p Days/tue
        $ mkdir -p Days/wed
        ...
        
Samalla menetelmällä loin myös muut viikonpäivän kansiot Days hakemiston alle. 

![Kuva5](https://user-images.githubusercontent.com/100162043/213856975-6b3f1c31-c72c-44b3-a70e-76b5b4ca7e7d.jpg)


Kuten kuvasta huomaa, kävin muutaman kerran tutkimassa, että lisääntyyhän hakemistoja Days hakemiston alle, ja lisääntyihän ne!

## Alahakemistojen alahakemistot

Nyt olen saanut viikonpäivät lisättyä Days hakemistoon, on aika lisätä jokaiselle viikonpäivälle sisältöä. Tässä kohtaa lisään jokaisen viikonpäivän alle
Fish Cat ja Horse kansiot. Avaan yksitellen viikonpäivät seuraavasti: 

        $ cd Days
        $ cd mon
        
Tämän jälkeen lisään esimerkin mon kansioon Touch komennolla Fish, Cat ja Horse tiedostot: 

        $ touch Fish
        $ touch Cat
        $ touch Horse.
        
Jonka jälkeen saamme kuvan mukaisen näkymän. 

![Uusikuva 5](https://user-images.githubusercontent.com/100162043/213857118-7bb0ba04-5537-4ca3-9820-85c002bb021e.jpg)


Huomattuani, että onnistuin, teen saman myös jokaiselle muulle viikonpäivälle!

## Lopputunnelmat

Onnistuneesta suorituksesta vielä kuva alla. Hetken aikaan pähkäilin ja kokeilin erilaisia variaatioita. Muun muassa touch menetelmää kokeilin jo luotuani Days
ja lisäämällä viikonpäivät touch menetelmän avulla. Tämähän ei tietenkään toiminut, sillä alakansioita viikonpäiville ei onnistuttu asettamaan. Pääasiana on 
erittäin hyvä fiilis mikä siunaantui onnistumisen ja kun viimein ymmärsin kuinka tässä kannattaa edetä. Mahtava ensi kosketus Terminaaliin!

![Kuva 6](https://user-images.githubusercontent.com/100162043/213857212-7480a6da-dafc-4179-a321-5f3af2059e3a.jpg)

       
