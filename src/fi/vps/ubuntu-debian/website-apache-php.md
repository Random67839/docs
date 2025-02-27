# Verkkosivut Apache2 ja PHP:llä

Tällä ohjeella pääset helposti alkuun verkkosivujen luomisessa virtuaalipalvelimella. Jos olet juuri hankkinut virtuaalipalvelimen, suosittelemme - että lukaiset [tulossa] ohjeen läpi ennen kun aloitat!  
  
## Haetaan päivitykset​

Ensin haemme mahdolliset päivitykset pakettienhallinnalle. Tämä onnistuu seuraavasti:  
`sudo apt update`  

![](https://cdn.bittivirta.fi/docimg/crisp/2120200522220843-6464d84a_1jjqaag.gif)

Päivityksen kesto riippuu siitä, että kuinka moni repositorio on päivittynyt sen jälkeen, kun viimeksi päivitit repositoriot.  

## Asennetaan Apache​

Asennetaan Apachen uusin versio, joka on Apache2. Tämä tapahtuu komennolla:  
`sudo apt install apache2 ` 

Asennin ilmoittaa vielä paketin koon ja pyytää vahvistamaan asennuksen. Kun asennin kysyy tätä, kirjoita konsoliin **Y** ja paina enter-näppäintä.  

Kun apache on asennettu, pääset palvelimesi verkkosivuille kirjoitamalla selaimen URL-osoitteeseen palvelimesi IP-osoitteen  

![](https://cdn.bittivirta.fi/docimg/crisp/2320200522233603-cb604678-la_i7br9a.png)

## Muokataan sivuston sisältöä​

Tässä vaiheessa kannattaa ottaa yhteyttä palvelimelle SFTP-yheyden avulla. Tähän voit käyttää esim. FileZilla- tai WinSCP-ohjelmistoa.  

Löydät sivuston oletussivun palvelimella sijaitsevasta kansiosta `/var/www/html`. Se sisältää oletuksena `index.html`-tiedoston, jonka voit poistaa ja ladata palvelimelle omat tiedostosi.  


## Asennetaan PHP​

Jos palvelinpuolella halutaan ohjelmoida jotakin, tarvitaan tähän esimerkiksi PHP. Moni ohjelmisto, kuten WordPress jonka voi asentaa sivustolle - tarvitsee PHP:n toimiakseen.  

PHP:sta löytyy useampia versioita, mutta tässä ohjeessa asennamme PHP:n repositorion uusimman version.

```bash
sudo apt install php #asennetaan PHP  
sudo apt install -y php-{gd,bz2,intl,mbstring,bcmath,mysql,zip} #asennetaan muutama paketti, joita tarvitaan yleisimmiten  
sudo apt install libapache2-mod-php #asennetaan apachen PHP-laajennus
```

Asentaja taas ilmoittaa asennuksen yhteydessä, että kuinka paljon ne vievät levytilaa. Hyväksytään asennus painamalla **Y** ja enter.  

Kun asentaja on asentanut paketit, voidaan tehdä tiedosto `test.php` kansioon `/var/www/html/`. Lisää tiedoston sisälle seuraava koodi:  
```php
<?php
phpinfo();
```

:::warning Huomaathan poistaa test.php-tiedoston sen tarkastelun jälkeen tai muuten rajoittaa sinne pääsyä, etteivät mahdolliset hyökkääjät saa palvelimestasi näitä tarkkoja palvelimesi tietoja.
:::

Tämän jälkeen siirry selaimella osoitteeseen [http://ip-osoite/test.php](http://ip-osoite/test.php). Jos näet vastaavanlaisen sivun, olet onnistunut PHP:n asennuksessa:  

![](https://cdn.bittivirta.fi/docimg/crisp/php_1e6jxnc.png)