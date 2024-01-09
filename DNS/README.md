Als aller erstes zur DNS einrichtung muss ein Windows Server eingerichtet werden. Dazu gebe ich noch in VmWare die nötigen Informationen an.

<img width="319" alt="Screenshot 2023-12-19 160147" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/29e318d8-74f0-46b3-a801-ceb2642f9ba3">

Das System wird eingerichtet und vorbereitet.

<img width="465" alt="Screenshot 2023-12-19 160206" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/02188dc2-0dcb-4b1f-97b2-43c71722ed14">

Nach der Installation wird der Servermanager gestartet. Dort gehe ich rechts neben der Fahne auf Manage und dann auf "Add Roles and Features".

![3Unbenannt](https://github.com/MaxHD00/M123_TMP/assets/31143468/8f44b7b2-4d61-4a3a-ad56-ce7de621c508)

Da wir den DNS hinzufügen wollen drücken wir auf die Rollen.

<img width="482" alt="4Screenshot 2023-12-19 160733" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/55bd72cb-b6de-4309-9644-38a7068e8c2f">

Und fügen anschliessend den DNS hinzu. Nach dem installieren ist hier kein Neustart notwenig.

<img width="482" alt="5Screenshot 2023-12-19 161141" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/2deb2d92-216c-435b-b09d-46c664894c40">

Der DNS ist eingerichtet, funktioniert und gibt keine Fehler aus.

<img width="173" alt="6Screenshot 2023-12-19 162509" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/10447ef4-fc94-403e-9f0b-385fe592458d">

Jetzt da der DNS installiert ist, muss dieser noch eingerichtet werden, sowie auch der Computer.

Ich beginne damit die Client und Server IP zu bestimmen. Sowie setze ich den DNS schon mal auf den Server.

Client:

<img width="296" alt="clientIPScreenshot 2024-01-09 152744" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/df727cc0-74af-46f1-9934-7ed6a7061b38">

Server:

<img width="439" alt="ServerIPScreenshot 2024-01-09 152811" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/5d70307c-7626-4c7f-924e-3dfd0c56b142">

Nachdem das gemacht wurde kann ich in die DNS Einstellungen gehen und eine Forward und Reverse zone hinzufügen.

<img width="453" alt="1Screenshot 2024-01-09 150522" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e2ab2e71-7b5e-42b7-bbcb-f4b4f4728d3e">

Hier klicke ich mich durch, gebe noch den namen "Sota" und stelle dann das erstellen fertig.
Bei den Forward DNS einstellungen ist es jetzt wichtig zwei neue Hosts zu erstellen. Einen für den Server, den anderen für den Client, dass das DNS funktioniert.

Server:

<img width="470" alt="2Screenshot 2024-01-09 150626" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/73cd7168-0fb6-4464-9f91-a6d48365a328">

Client:

<img width="461" alt="3Screenshot 2024-01-09 150651" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/2497a2eb-d3d1-429d-b71c-bfb097bd08b5">

Bei den Reverse DNS Einstellungen müssen diese auch angegeben werden. Allerdings anders als bei den Forward Einstellungen. Hier kann ich nämlich einfach die Forward Einstellung angeben und der rest wir von selbst eingestellt.

<img width="464" alt="4Screenshot 2024-01-09 150743" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e3dc9e36-70da-431b-8e8b-4e5c38a8d5fa">

Nachdem das alles eingerichtet und eingestellt wurde teste ich erstmal den Pingaustausch zwischen Server und Client.
Dieser brachte einige komplikationen. Aber nach eine weile funktionierte auch das.

Client:

<img width="269" alt="PingClientScreenshot 2024-01-09 153029" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/cbf7f2b8-2b12-458e-863f-38be0c564183">

Server:

<img width="284" alt="PingserverScreenshot 2024-01-09 152955" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/5717ef77-1b83-4559-9abd-c45fbc5aec34">

Jetzt sollte mich nichts mehr dran hindern den DNS zum laufen zu bringen. Und tatsächlich. Direkt nach dem lösen des Ping Problems funktionierte der DNS lookup auch.

<img width="200" alt="ResoultatScreenshot 2024-01-09 152846" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/56835f01-f3c5-4e88-a8b1-a1796ce6b98d">

Als weiteren Test habe ich dann noch eine externe Webseite wie google über den nslookup angesprochen, was auch funktioniert hat:

<img width="235" alt="nslookupgoogleScreenshot 2024-01-09 153441" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/1c9b42bf-7746-456c-9124-582190ff2a45">
