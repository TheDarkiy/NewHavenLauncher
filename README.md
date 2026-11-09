NewHavenLauncher
================

Version 1.0.0

Inhalt dieses Release
---------------------
- NewHavenLauncher.exe  - Der Launcher
- clientcfg.json        - Lokale Einstellungen; wird bei Bedarf neu erstellt
- logs\                 - Pro Start wird hier eine Protokolldatei abgelegt

Start
-----
1. Starte NewHavenLauncher.exe.
2. Stelle sicher, dass FiveM installiert ist und eine Internetverbindung besteht.
3. Wenn der Server online ist, kannst du im Launcher auf „Beitreten“ klicken.

Der Launcher sucht FiveM.exe automatisch. Wird FiveM gefunden, startet der
Launcher FiveM und versucht anschließend, mit dem New-Haven-Server zu verbinden.
Der Launcher-Ordner muss beschreibbar sein, damit Einstellungen und Logs
gespeichert werden können.


FiveM-Pfad und Fenstergröße
--------------------------
Die Datei clientcfg.json liegt neben der EXE. Beim ersten Start werden
Standardwerte angelegt:

{
  "WindowWidth": 1280,
  "WindowHeight": 720,
  "FiveMPATH": ""
}

Ist FiveMPATH leer, versucht der Launcher, FiveM.exe automatisch zu finden.
Falls die automatische Suche nicht funktioniert, trage dort den vollständigen
Pfad zu einer vorhandenen FiveM.exe ein, zum Beispiel:

  "FiveMPATH": "C:\\Games\\FiveM\\FiveM.exe"

WindowWidth und WindowHeight legen die Fenstergröße fest. Beide Werte müssen
positive ganze Zahlen sein. Schließe den Launcher vor dem Bearbeiten der Datei.
Ungültige JSON-Daten oder ungültige Werte verhindern den Start.

Protokolle und Hilfe bei Problemen
----------------------------------

Für jeden Start wird eine neue .log-Datei im Ordner logs neben der EXE erstellt.
Wenn der Launcher oder der Spielstart nicht funktioniert, prüfe, ob FiveM.exe
vorhanden und erreichbar ist und ob der Launcher-Ordner beschreibbar ist.
Die neueste Log-Datei enthält technische Details, die du zur Fehlersuche
weitergeben kannst.

Serverstatus und Beitreten benötigen eine Internetverbindung. Ist der Server
offline oder nicht erreichbar, bleibt die Beitreten-Schaltfläche deaktiviert.
