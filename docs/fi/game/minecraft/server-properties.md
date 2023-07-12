# server.properties -asetustiedosto
Tässä artikkelissa ohjeistetaan palvelimen asetuksien muuttamista. Asetustiedoston löydät Gamepanelissa, kun navigoit: Palvelimesi » Files » server.properties

## Asetuksien tyypit:​
[tulossa]

## Asetuksen selitykset:​
[tulossa]

## Oletusasetustiedosto​
Palvelimen IP-osoite ja portti vaihtelee oletusasetuksissa. Voit jättää asetuksen halutessasi tyhjäksi, tai joksikin muuksi arvoksi, sillä siihen korjataan aina palvelimesi osoite ja portti palvelimen käynnistyessä.

```proerties
#Minecraft server properties
#(File modification date and time)
enable-jmx-monitoring=false
rcon.port=25575
level-seed=
gamemode=survival
enable-command-block=false
enable-query=false
generator-settings={}
enforce-secure-profile=true
level-name=world
motd=A Minecraft Server
query.port=25565
pvp=true
generate-structures=true
max-chained-neighbor-updates=1000000
difficulty=easy
network-compression-threshold=256
max-tick-time=60000
require-resource-pack=false
use-native-transport=true
max-players=20
online-mode=true
enable-status=true
allow-flight=false
initial-disabled-packs=
broadcast-rcon-to-ops=true
view-distance=10
server-ip=
resource-pack-prompt=
allow-nether=true
server-port=25565
enable-rcon=false
sync-chunk-writes=true
op-permission-level=4
prevent-proxy-connections=false
hide-online-players=false
resource-pack=
entity-broadcast-range-percentage=100
simulation-distance=10
rcon.password=
player-idle-timeout=0
force-gamemode=false
rate-limit=0
hardcore=false
white-list=false
broadcast-console-to-ops=true
spawn-npcs=true
spawn-animals=true
function-permission-level=2
initial-enabled-packs=vanilla
level-type=minecraft\:normal
text-filtering-config=
spawn-monsters=true
enforce-whitelist=false
spawn-protection=16
resource-pack-sha1=
max-world-size=29999984
```

:::details Lähteet
Official Minecraft Wiki: Server.properties. Päivitetty 9.1.2023.<br>
Saatavissa: https://minecraft.gamepedia.com/Server.properties [Käytetty lähteenä 16.1.2023]
:::