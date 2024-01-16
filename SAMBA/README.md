Unsere Aufgabe war es einen Samba Server auf einem Linux Gerät zu installieren.
Weil ich es grade zur Hand hatte nutzte ich Linux Mint.

"sudo apt update" zum updaten aller packages.

<img width="365" alt="1 apt update Screenshot 2024-01-16 135443" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/3f190721-5a0e-4b8a-8b89-307c967c2d4e">

"sudo apt install samba" zum installieren von Samba.

<img width="388" alt="2 install samba Screenshot 2024-01-16 135645" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/b2e2c8a8-a44d-4cf9-8a8b-bfb91a35b26a">

"systemctl status smbd --no-pager -l" zum überprüfen, ob der Server läuft.

<img width="513" alt="3 systemctl status smbd --no-pager -l" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e8894740-0a44-4a12-a3b8-316ab1772f44">



<img width="425" alt="4 sudo systemctl enable --now smbd" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e97565f7-dd94-4549-bae9-b5507a2d24bb">



<img width="158" alt="5 sudo ufw allow samba" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/7d4d5ab1-56f5-4780-b2e1-d79ed1e4fced">

Der Nutzer wird eingerichtet, welcher sein Ordner freigeben will.
Hier wird dann Nutzername und Passwort eingetragen. Hier: Mint als Username und max als passwort.

<img width="275" alt="6 Add your user to the Samba group" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/725bcd87-3296-4f11-844d-4c5a97a76d8d">

Nachdem Samba eingerichtet wurde, muss ich nur noch den Ordner sharen und die Rechte verteilen.

<img width="434" alt="7 file sharing Screenshot 2024-01-16 141557" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/2d1b405b-2257-46a1-a432-1f29a0f4c289">



<img width="409" alt="8 permissions Screenshot 2024-01-16 141629" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/18554365-ca5b-4fa1-8b90-0c109d1989e8">



<img width="61" alt="9 Icon Screenshot 2024-01-16 141732" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/e9d8b76b-89e4-4061-a24b-7075e6a0d884">

Ab jetzt gehts zum Windows client, wo ich einfach nur die IP-Adresse eingeben muss.

<img width="374" alt="10 Windows Screenshot 2024-01-16 142545" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/cb925777-4c8e-4e98-9535-9676c6bdad97">

Und dann hat auch alles funktioniert, nachdem ich die Anmeldedaten angegeben habe.

<img width="776" alt="11 fertig Screenshot 2024-01-16 142831" src="https://github.com/MaxHD00/M123_TMP/assets/31143468/69d42e33-f4ae-4219-9e84-2cf9aeebbe30">