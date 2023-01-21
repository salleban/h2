# h2
Linux terminal

# Termial

Aloitus käy mukavasti. Huomaan Virtuaalikonetta käynnistäessä saavani virheen, että tiedostot puuttuvat. Eli asentelen uudelleen VirtualBoxin..

Sitten itse aiheeseen. Lähdin rakentamaan hakemistoa touch menetelmällä. Mutta ensin avasin Terminalin ja katsastelin olemassa olevat hakemistot läpi. 

-KUVA-

Käytin pwd hakua selvittääkseni, missä hakemistossa olen ja tämän jälkeen selvitin ls hakua selvittääkseni mitä Home kansion alta löytyy. 

## Hakemisto

Hakemiston nimeäminen ja luominen tapahtuu mkdir komennon avulla. Kirjoittamalla mkdir ja perään haluamasi nimi hakemistolle, syntyy hakemistokansio. Esimerkiksi:

        $ mkdir Days 
        
Nähdäksesi onnistuiko hakemiston luominen kirjoita:

        $ ls
        
-KUVA-

Näin huomaan luoneeni Days hakemiston muiden joukkoon. 

## Hakemiston alakansiot

Seuraavan vuorossa on lisätä Days hakemistoon kansioita. Tyhjennetään tässä vaiheessa terminaali painamalla ctrl + L. 
Katsoin kirjoittamalla pwd, että olenko varmasti Home kansiossa tyhjennettyäni terminaalin ja huomasin olevani edelleen uudella luomallani Days kansiossa. 

-KUVA- 

Hakemiston saa ns. nollattua kirjoittamalla terminaaliin cd ~. Nyt kirjotan uudestaan pwd ja huomasin olevani takaisin home kansiossa. 

Seuraavaksi luokdaan Days hakemiston alle viikonpäivän hakemistot. Tämä tapahtuu kirjoittamalla: 

        $ mkdir -p Days/mon

Katsoammeksemme toimiko tämä komento, kirjoitetaan: 

        $ cd Days
        $ ls
        
Ja huomaan kuvan mukaisesti, että mon niminen hakemisto on luotu Days hakemiston alle. 

-KUVA-



        $ mkdir -p Days/tue
        $ mkdir -p Days/wed
        ...
        
Samalla menetelmällä loin myös muut viikonpäivän kansiot Days hakemiston alle. 

-KUVA-

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

-KUVA-

Huomattuani, että onnistuin, teen saman myös jokaiselle muulle viikonpäivälle!

## Lopputunnelmat

Onnistuneesta suorituksesta vielä kuva alla. Hetken aikaan pähkäilin ja kokeilin erilaisia variaatioita. Muun muassa touch menetelmää kokeilin jo luotuani Days
ja lisäämällä viikonpäivät touch menetelmän avulla. Tämähän ei tietenkään toiminut, sillä alakansioita viikonpäiville ei onnistuttu asettamaan. Pääasiana on 
erittäin hyvä fiilis mikä siunaantui onnistumisen ja kun viimein ymmärsin kuinka tässä kannattaa edetä. Mahtava ensi kosketus Terminaaliin!

-KUVA-
       
