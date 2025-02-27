# Verkkotunnuksen lisääminen (Plesk/Bittivirta)
## 1. Haetaan IP-osoite ja portti​
Kirjaudu Gamepaneliin osoitteessa https://gamepanel.fi/, valitse palvelin jolle teemme osoitteen. Kopioi IP-osoite sekä portti.

![](https://cdn.bittivirta.fi/docimg/crisp/image_1pifx1h.png)

## 2. Luodaan tietue Pleskissä
Kirjaudu asiakasalueelle ja siirry "Minun..." » "Palveluni" » (Valitse webhotellisi, jossa haluamasi verkkotunnuksen hallinta sijaitsee):
![](https://cdn.bittivirta.fi/docimg/crisp/screenshot-2022-08-18-at-15472_1i5d2ku.png)

​Valitse "Kirjaudu Pleskiin":
![](https://cdn.bittivirta.fi/docimg/crisp/screenshot-2022-08-18-at-17083_1cvd1xr.png)

Valitse verkkotunnuksesi ja valitse "DNS-asetukset":
![](https://cdn.bittivirta.fi/docimg/crisp/screenshot-2022-08-18-at-17111_142xl9q.png)

Valitse "Lisää tietue"-painike:
![](https://cdn.bittivirta.fi/docimg/crisp/screenshot-2022-08-18-at-17135_1l3n2hh.png)

Täytä tiedot seuraavasti (selitykset alempana):
![](https://cdn.bittivirta.fi/docimg/crisp/screenshot-2022-08-18-at-17182_d971ko.png)

* **Tietuetyyppi** on `SRV`.
* **Palvelun nimi** on `minecraft`,
* **Protokolla** on `TCP`.
* **Toimialueen nimi**-kenttään voit asettaa minkä tahansa tekstin, jonka haluat - jolla palvelimelle liitytään (jos haluat, että etuliitettä ei ole, jätä kenttä tyhjäksi). Kuvan esimerkin mukaan osoitteeksi tulee mc.sirkulaattori.fi.
* **Port** on palvelimesi portti, niin kuin tässä tapauksessa _25574_.
* **Kohdeisäntä** on pelipalvelimesi osoite ilman porttia, joka tässä tapauksessa on _g5.bitti.gg_.
* **TTL**, **priority** ja **weight** ovat vapaasti valittavissa olevia kenttiä. Pleskin tarjoamat oletukset ovat hyvät arvot.

Halutessasi voit lisätä `SRV` -tietueita lisää niin monta, kuin tarvitset.

**Onnea pelipalvelimen kehitykseen!**
