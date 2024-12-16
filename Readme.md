# SPT Setup

Das wichtigste zuerst SPT installieren:
Anforderungen

Escape From Tarkov (siehe Registerkarte „Versionen“ für unterstützte Spielversionen)

1. [.NET Framework 4.7.2](https://download.visualstudio.microsoft.com/download/pr/51bc18ac-0594-412d-bd63-18ece4c91ac4/90b47b97c3bfe40a833791b166697e67/windowsdesktop-runtime-8.0.3-win-x64.exe)

2. [.NET Runtime 8](https://go.microsoft.com/fwlink/?linkid=874338)

Installation

*Verwenden das [automatische Installationsprogramm](https://ligma.waffle-lord.net/SPTInstaller.exe). Die manuelle Installation wird offiziell nicht mehr unterstützt. 

Mit automatisches Installationsprogramm:

1. Neuen Ordner erstellen auf der Festplatte (muss nicht auf der gleichen sein aber bitte nicht in den Tarkov Ordner direkt).
2. Starte das automatische Installationsprogramm, es sollte so aussehen nur mit einem Grünen Feld ganz unten! [Unbenannt4](https://github.com/user-attachments/assets/89304b0b-6dee-4a0a-81fd-03d263e62f0a).
3. Nun kannst du es Installieren und ganz viel Spaß haben. :)

Ohne automatisches Installationsprogramm:

Das automatische Installationsprogramm geht nicht so wie bei mir oder du willst einfach besonders sein? Kein Problem es geht auch Manuel.

1. Neuen Ordner erstellen auf der Festplatte (muss nicht auf der gleichen sein aber bitte nicht in den Tarkov Ordner direkt).
2. Aus dem Original Ordner Tarkov komplett Kopieren in dem du STRG+A und dann ohne die Maus zu benutzen STRG+V drückst.
3. Inzwischen können wir uns [SPT](https://spt-releases.modd.in/SPT-3.10.3-33420-42b3d7a.7z) holen.
4. Danach einfach alles im SPT Ordner entzippen und fertig viel Spaß. :)

Wie Starte ich es?
1. Starte Server.exe
2. Starte Launcher.exe
3. Launcher > Neues Konto erstellen
4. Launcher > Spiel starten.

SPT ist nicht von mir hier die [github Seite](https://github.com/sp-tarkov) und die [Offizielle seit](https://sp-tarkov.com/) für SPT und die im Modpack benutzten Mods

# Fika Setup

Jetzt kommen wir zum Teil, das uns Koop spielen lässt, und zwar [Fika](https://github.com/project-fika/Fika-Documentation).
In den nächsten schritten, werde ich erklären wie du ja du eine eigene Lobby machen kannst und auch anderen Joinen kannst.
Ich bin mir sehr sicher, dass du das schafft.

Was brauchen wir:

1. Als Laufwerk eine SSD es geht jedoch auch eine HDD es ist jedoch die SSD zu empfählen
2. Als Host eine Internetverbindung die bei ungefähr 20Mb/s ist.
3. Verdammt nochmal SPT installiert!!!
4. CPU: i7 8700k / Ryzen 7 2700x
5. GPU: GTX 1060 / RX 580
6. 16-32GB Ram 32GB ist jedoch zu empfehlen

Schritte als Host:
Das ist die VPN Variante mit der [radmin](https://download.radmin-vpn.com/download/files/Radmin_VPN_1.4.4642.1.exe) VPN 

1. Als erstes Lade dir [FikaUtils](https://github.com/Lacyway/FikaUtils/releases/download/v1.0/FikaUtils.zip) herunter
2. Schmeiß sie in den SPT Ordner und öffne sie, es sollte so aussehen: ![Unbenannt3](https://github.com/user-attachments/assets/bc4a2b44-6762-4e95-9e85-c024631d0597)
* Wir öffnen damit die Firewall, um den Zugriff für andere Spieler zuzulassen bitte habt immer euren ANTI Virus an und seit euch im Klaren, was ihr Installiert.
3. Nun drücken wir 1 und enter

*Ich hoffe ich muss euch nicht erklären wie ihr die VPN Benutzt oder?
*Gut werde ich auch nicht.

4. Laden das neueste [Fika-Plugin](https://github.com/project-fika/Fika-Plugin/releases/download/v1.0.6.0/Fika.Release.1.0.6.0.zip) und den neuesten [Fika-Server-Mod](https://github.com/project-fika/Fika-Server/releases/download/v2.3.3/fika-server.zipherunter)
5. Navigieren zu deiner SPT-Installation und extrahieren den Inhalt des Archivs in den Ordner
6. Starten den SPT.Server.exe einmal, damit es die Konfigurationsdateien für Fika generiert, und schließen Sie es dann wieder
7. Gehe zurück zum Hauptordner, navigieren zu SPT_Data\Server\configs und öffnennhttp.json

*Beispiel IP ![Unbenannt6](https://github.com/user-attachments/assets/23c2d503-f355-4a16-ad38-bd115ab46c59)

8. Änder die IP und BackendIp zur VPN-IP, speicher dann die Datei und schließe sie.
9. Navigiere zu user\mods\fika-server\assets\configs und öffnen fika.jsonc
10. Ändern die Einstellungen nach deinem Wunsch.
    useBtr: ob der BTR beim Spielen von Streets spawnen soll oder nicht
    FriendlyFire: ob Friendly Fire aktiviert sein soll oder nicht
    dynamische VExfils: Skaliert automatisch die maximale Spieleranzahl von Fahrzeug-Exfils mit der Anzahl der Spieler im Raid
    AllowFreeCam: Ermöglicht Spielern das freie Umschalten der kostenlosen Kamera während Raids
    giftedItemsLoseFIR: wenn gesendete Artikel ihren FiR-Status verlieren sollten

11. Starten den SPT.Server.exe und warte, bis der Ladevorgang abgeschlossen ist.

*So sollte es aussehen, wenn es in Schritt 7 gelungen ist, mit der Beispiel-IP zu beginnen: 

![Unbenannt5](https://github.com/user-attachments/assets/02275d58-3d18-480a-9a1a-a600e157cfba)

12. Starte den SPT.Launcher.exe, klicke auf „Einstellungen“ und aktivieren den Entwicklermodus
13. Ändere das URL-Feld so, dass es deine VPN-IP widerspiegelt. z.b.: http://20.20.56.73:6969 
14. Starten Nun das Spiel und stelle nach der Erstellung deines Kontos sowohl Force IP als auch Force Bind IP auf deine eigene, persönliche VPN-IP ein. Du findest diese, indem du im Hauptmenü auf F12 klicken.


Client mit einem VPN

1. Aktuellsten Fika Release herunterladen
2. Navigiere zum SPT Ordner und entpacke den Inhalt der eben heruntergeladenen Datei in diesen
3. Starte Aki.Launcher.exe und klicke auf 'Settings'
4. Gib im URL Feld die VPN IP ein. z.b.: http://20.20.56.73:6969 (achte darauf, dass keine führenden / hinter dem Port stehen)
5. Wenn der Client Ingame die Session erstellen soll müssen alle Verbindungen (Öffentlich und Privat) freigegeben werden wenn die Aufforderung von der Windows Firewall erscheint






