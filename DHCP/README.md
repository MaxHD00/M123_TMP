

# DHCP

### Auftrag 1

How to DHCP in Fillus auslesen:
Fillus wieder installieren, DHCP Server sowie alle anderen Komponennten zusammenverbinden.
Bei Client 1 & 2 DHCP zur Konfiguration freigeben.
Client 3 bleibt erstmal unverändert.
Beim DHCP Server DHCP einrichten.
Sicher gehen, dass in den Grundeinstellungen die Unter und Obergrenze 192.168.0.150-170 eingerichtet ist.
Unter Statische Adresszuweisung für den Client 3 die Mac sowie IP-Adresse des Client 3 eintragen.
Anschliessend DHCP einschalten:


<img src="https://github.com/MaxHD00/Maumau/assets/31143468/6358769c-dcda-4ce2-a8dc-5bf737f8cc8a" width="200" height="40"  alt=""/>

Simulation starten und überprüfen, wie Server und Client sich austauschen.

<img src="https://github.com/MaxHD00/Maumau/assets/31143468/ac16ad57-7c04-4c15-bd1e-f39c6758304a" width="800" height="500" alt="" />


---

### Auftrag 2

Der erste schritt forderte, wie der DHCP-Server die IPv4 an alle lokalen Netzwerke einbindet.
Diese werden über das terminal auch CLI genannt von Router erledigt.
Für welches Subnetz ist der DHCP Server aktiv?:

<img src="https://github.com/MaxHD00/Maumau/assets/31143468/4d6013cd-0d95-48cf-b55d-4f954c41a548" width="800" height="150" alt="" />


Welche IP-Adressen ist vergeben und an welche MAC-Adressen?:
<img src="https://github.com/MaxHD00/Maumau/assets/31143468/362ccedc-26b4-4819-9412-3c78b613d96a">

In welchem Range vergibt der DHCP-Server IPv4 Adressen?:
<img src="https://github.com/MaxHD00/Maumau/assets/31143468/c5e1c589-52ad-45dc-9c49-a731f1b4cf54">

Was hat die Konfiguration ip dhcp excluded-address zur Folge?
Bestimmte Ip-adressen können damit ausgeschlossen werden.
Das hilft um IP-Konfligte zu lösen, Netzwerkkonfikte oder auch zur einfachen Konfiguration.

Wie viele IPv4-Adressen kann der DHCP-Server dynamisch vergeben?

254
