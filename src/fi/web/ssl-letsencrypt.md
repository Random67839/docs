---
title: Ilmainen HTTPS/SSL
description: Ilmainen SSL-sertifikaatti Let's Encryptin avulla
---

![](https://cdn.bittivirta.fi/docimg/crisp/image_4fwtl3.png)

SSL-sertifikaatti, eli verkko-osoitteen edessä näkyvä http-etuliitteen sijaan käytössä oleva https-etuliite on nykyään lähestulkoon pakollista olla jokaisella sivustolla. Näin ollen Bittivirta tarjoaa kaikille webhotellipaketeille ilmaisen Let's Encrypt-sertifikaatin, joka on helppo ottaa käyttöön ja on jatkossa täysin automaattinen.

Sertifikaatin pitäisi olla oletuksena käytössä, mutta joskus sertifikaatin asennus sivustoa lisätessä ei automaattisesti onnistu, kun verkkotunnus on uusi, nimipalvelimet ovat juuri vaihtuneet tai jokin muu pikkutekijä on tähän vaikuttanut.

# 1. Kirjaudu Pleskiin​
Avaa Plesk asiakasalueella OneClick-kirjautumisella tai kirjaudu Pleskiin osoitteessa [https://plesk.bitivirta.cloud/](https://plesk.bittivirta.cloud/)

# 2. Valitse verkkotunnus jota hallitset ja klikkaa SSL/TLS-varmenteet​
![](https://cdn.bittivirta.fi/docimg/crisp/image_1k8tj0o.png)


# 3. Valitse "Install a free basic certificate provided by Let's Encrypt"​
![](https://cdn.bittivirta.fi/docimg/crisp/image_1dokdof.png)

# 4. Valitse tarvitsemasi suojatut alueet​
Jos et tiedä tarkemmin, mitä tarvitset tai haluat, valitse kuvassa merkityt kohteet ja klikkaa "Hanki se ilmaiseksi":
![](https://cdn.bittivirta.fi/docimg/crisp/image_1nlw03s.png)

# 5. Paranna suojausta​
Halutessasi ottaa vielä pari ekstra-askelta parempaa tietoturvaa kohden, ota HSTS ja OSCP-nidonta käyttöön seuraavista asetuksista:

:::danger Huomaa!
Tee nämä toimenpiteet vasta, kun olet varmistanut, että sivustosi toimii https-yhteydellä.
:::

![](https://cdn.bittivirta.fi/docimg/crisp/image_1k9a0l9.png)

Saadessasi nämä askeleet valmiiksi, sivustosi asiakkaiden tiedot ovat salattuja asiakkaan ja palvelimen välillä! Onnea sivuston perustamiseen!