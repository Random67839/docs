---
order: 1
---
# Tiedostojen hallinta

Voit hallita tiedostojasi joko selaimessa tai tietokoneeltasi SFTP-yhteyden yli.

## Tiedostojen hallinta selaimessa

:::warning Huomaa!
Suurien tiedostojen hallinta (yli 100MB) selaimessa ei ole mahdollista. Suurempien tiedostojen hallintaan voit käyttää SFTP-yhteyttä.
:::

1. Kirjaudu Gamepaneliin
2. Valitse palvelin, jonka tiedostoja haluat muokata
3. Valitse "Files"
    ![Tiedostojen hallinta](https://cdn.bittivirta.fi/docimg/en/game-servers/gamepanel/files.png =500x)
4. Muokkaa tiedostoja

Lisää ohjeita tiedostojen hallinnasta sivulla [Selaimen tiedostomuokkain](/pelipalvelimet/gamepanel/tiedostomuokkain.html).

## Tiedostojen hallinta SFTP-yhteydellä

SFTP, eli Secure File Transfer Protocol on SSH-suojattu FTP:n tapainen tiedostojen siirto- ja hallintaprotokolla. SFTP-yhteyden avulla voit hallita palvelimen tiedostoja tietokoneeltasi.

Pelipalvelimilla ei ole lainkaan tavallista FTP-protokollaa, sitä ei voi käyttää palvelimemme tiedostojen hallintaan. SFTP on täysin vastaava kuin FTP, mutta sen tietoliikenne on salattu.

Tiedostoja voidaan hallita muutamallakin eri tavalla. Valitse itsellesi mieluinen tapa käsitellä tiedostoja, voit kokeilla eri tapoja ja katsoa mikä on sinulle sopivin.

<div style="display:flex;align-items:start;flex-wrap:wrap;">
<div style="margin-right:4rem;">

### SFTP-ohjelmistoja

#### <icon icon="fa:windows" width="13px"/> Windows

* [FileZilla](desktop/windows/sftp/filezilla)
* [WinSCP](desktop/windows/sftp/winscp)
* Cyberduck
  
#### <icon icon="fa:apple" width="13px"/> macOS

* FileZilla
* Transmit (maksullinen, mutta paras)
* Cyberduck
#### <icon icon="fa:linux" width="13px"/> Linux

* FileZilla

</div>
<div>

### Tekstieditorit

#### <icon icon="fa:windows" width="13px"/> Windows

* [Visual Studio Code](desktop/windows/tiedostomuokkaimet#visual-studio-code)
* [Notepad++](desktop/windows/tiedostomuokkaimet#notepad)
* [Sublime Text](desktop/windows/tiedostomuokkaimet#sublime-text)

#### <icon icon="fa:apple" width="13px"/> macOS

* Visual Studio Code
* Sublime Text

#### <icon icon="fa:linux" width="13px"/> Linux

* Visual Studio Code
* Vim

</div>
</div>

## SFTP-yhteyden luominen

SFTP-yhteyden luomiseksi tarvitset palvelimen osoitteen, portin, käyttäjänimen ja salasanan.
* Palvelimen osoite on aina mallia `gX.bitti.gg` tai `hX.bitti.gg`, missä X on sen palvelimen numerotunniste, missä pelipalvelimesi sijaitsee
* Palvelimen portti on aina `2022`
* Käyttäjänimi jokaiselle Gamepanelissa olevalle pelipalvelimelle on eri, mallia Gamepanel-käyttäjänimesi, piste ja palvelimen tunniste
* Salasana on Gamepanel-salasanasi, jonka voit tarvittaessa resetoida [täällä](https://gamepanel.fi/auth/password).

Näet palvelimen kirjautumistiedot kätevästi myös Gamepanelista palvelimen sivulla Settings-välilehdeltä:

1. Valitse "Settings"
2. Palvelimen STP-osoite, joka sisältää myös portin. Jotkin ohjelmat osaavat ottaa myös portin asetuksiin, kun liität tämän ohjelmiston Host-/isäntä-kenttään
3. Käyttäjäsi palvelinkohtainen käyttäjänimi
4. Palvelimen osoite, joka ei sisällä porttia

![Palvelimen Gamepanel-asetukset](https://cdn.bittivirta.fi/docimg/en/game-servers/gamepanel/settings.png)
