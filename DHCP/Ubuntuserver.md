
Unsere Aufgabe war es nun einen UbuntuServer auzusetzen. Dazu habe ich eine neue vm erstellt, ein weiteren netzwerkadapter installiert und dann die ubuntuserver iso gestartet.

<img width="461" alt="Screenshot 2023-12-12 142818" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/3e679ab3-609c-406c-a511-1ba7a94cd2d5">

Als erstes frage mich Ubuntu, ob er die neusten Updates installieren sollte. Ich stimmte das zu und er startete die Updates.

<img width="668" alt="updateScreenshot 2023-12-12 143107" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e1160993-b8c7-479b-8687-d34b8dc64bc6">


Danach wurde gefragt, wie genau der Server installiert werden soll. Hier wählte ich den Standard.

<img width="654" alt="3choose installScreenshot 2023-12-12 143134" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/db41e11d-6c04-4921-bf06-b61caf8e5e6b">


Nun kam ich zum wichtigen Teil. Anstatt das später in einer file zu ändern kann ich auch ganz einfach bei der installation die Network daten richtig einstellen. Dies tat ich.

<img width="635" alt="4networkScreenshot 2023-12-12 143250" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/26aa8a82-90e2-4ddd-b498-e891a78dc87a">

Damit hatte ich jetzt eine Dynamische NAT karte und eine Statische Netzwerkkarte drin. 

<img width="299" alt="5staticScreenshot 2023-12-12 143325" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/cc0e581d-386f-41d6-9840-ef18ccd392bc">

Jetzt ging es noch drum die login daten sowie die namen festzulegen. Hier schrieb ich einfach ausser beim Servername überall "max".

<img width="634" alt="6username2Screenshot 2023-12-12 143615" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/a7563b4e-f5e3-456a-b34f-3dc3d7641764">
 
Und jetzt war es zeit für die Installation.

Die leider fehlgeschlagen ist und ich alles nochmal machen musste.

<img width="631" alt="7Screenshot 2023-12-12 143650" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/55bb23c8-a6b2-4fa9-bdab-ee3bfa71258e">

Und das beim zweiten mal auch wieder...

Sodass ich ab jetzt mit einer anderen Person zusammengearbeitet habe. Die folgenden Bilder stammen von einem anderen computer:


Dort hat die installation funktioniert. So haben wir also erstmal alles richtig konfiguriert:

<img width="440" alt="aaconfigure_ubuntudhcp_configuration" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/eb9a6ea3-59e7-49fd-b142-23b537701eea">

Das gleiche auch bei den DHCP configurationen:

<img width="410" alt="aaconfigure_ubuntudhcp_dhcpd-config" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/b07a6af9-4648-4f15-a894-ee3f1024b0de">

Wir waren zuversichtlich, allerdings hatten wir noch einen Fehler.
Der Fehler war es, dass wir die falsche Netzmaske angegeben haben.

<img width="493" alt="aaconfigure_ubuntudhcp_troubleshooting_1" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/3b34c8b8-c511-447b-ab87-d6076c97f0c4">

Nachdem wir den Fehler behoben haben, ist es uns gelungen den DHCP server komplett zum laufen zu bringen.


<img width="454" alt="aaconfigure_ubuntudhcp_troubleshooting_1s" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/565f8775-fe1a-4503-aa81-b0c0288b8b6f">

Das Windows OS hat dann die richtige IP Adresse angezeigt.

<img width="341" alt="aaconfigure_ubuntudhcp_proof 1" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/bcfd0120-d160-4a37-82ce-8186a3f5985a">

Und die leases configurations waren auch korrekt.

<img width="308" alt="aaconfigure_ubuntudhcp_leases 1" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/b01f008d-8d62-46fe-91ee-09315e579098">
