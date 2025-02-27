# Palvelimen "wipe"​

Tässä artikkelissa ohjeistetaan palvelimen alustamisessa. Kohdekansion löydät Gamepanelissa, kun navigoit:

Palvelimesi » _(valitse haluamasi palvelin)_ » Tiedostojen hallinta » server » rust

:::danger Ennen kuin alat poistamaan mitään, ota kaikesta tärkeästä ja tarpeellisesta varmuuskopiot! Näihin luokitellaan esimerkiksi Oxidemodin lisäosat ja niiden konfiguraatiot.
:::

Tutustu Oxidemodin asentamiseen täältä: [tulossa]

# Kuinka suoritan pelkälle kartalle wipen?​

Poistaaksesi kartan, sinun tulee olla kansiossa `/server/rust` . Valitse seuraavat tiedostot ja poista ne:
* `proceduralmap.#.#.#.map`
* `procefuralmap.#.#.#.sav`

![](https://cdn.bittivirta.fi/docimg/crisp/image_192otey.png)

Poistamalla pelkän kartan jätät pelaajille kaikki tavarat inventoryyn sekä pelaajien blueprintit eivät katoa.

Poistettua karttaa ei pysty palauttamaan edes varmuuskopiolla.

Jos haluat, että uusi karttasi näyttää erilaiselta wipen jälkeen, vaihdathan palvelimen seed -arvoa, jolloin kartta generoituu eri näköiseksi.

Pystyt vaihtamaan palvelimen seed -arvoa käynnistysparametreista käsin. Lue lisää täältä: [tulossa]

# Kuinka poistan palvelimelta pelaajadatan (blueprintit + inventoryt)?​

Poistaaksesi pelaajadatan, sinun tulee olla samassa kansiossa kuin ylempänä on ohjeistettuna.

Valitse seuraavat tiedostot ja poista ne:
* `player.blueprints.#.db`
* `player.deaths.#.db`
* `player.identities.#.db`
* `player.states.#.db`
* `player.tokens.db`

![](https://cdn.bittivirta.fi/docimg/crisp/image_1nfgnrx.png)

Jos haluat poistaa pelaajadatan (inventoryn), mutta jättää blueprintit niin älä koske `player.blueprints.#.db` -tiedostoon.

Pystyt palauttamaan pelaajadatan, jos olet ottanut itse varmuuskopion.

# Mitä muut kansion tiedostot ovat?​

Kansiossa on muitakin tiedostoja. Koske niihin omalla vastuulla. Lisäksi "cfg" -kansiosta löytyy bannilista ja muutamia muita tiedostoja.