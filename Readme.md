# ANLEITUNG

## Emulator installieren

1. Ordner erstellen
2. Ordner öffnen
3. SHIFT + Rechtsklick in den Ordner
4. Powershell Fenster hier öffnen
5. Script unten kopieren
6. Einfügen in Powershell (Macht man einfach mit einem rechtsklick)
7. Warten, wenn Windows nach berechtigung fragt, akzeptieren
8. Installer startet, installation durchführen
9.  Im Ordner wurde alles erstellt, kann jetzt verschoben werden


*Bei Problemen während der Installation, bitte bei Ihrem örtlichen Hannes melden.*


  **Done**

###### Script:
```
Set-ExecutionPolicy Bypass -Scope Process -Force;
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;
iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/TestRunnerSRL/bizhawk-co-op/master/bizhawk-co-op.ps1'))
```

## Emulator konfigurieren
Euer Emulator wurde installiert, zu finden unter *BizHawk-2.3\EmuHawk.exe*

1. Gehe zu  ```Config -> Customize -> Advance``` 
2. Unten sind Optionen für *Lua Core*
3. Wähle ```Lua+LuaInterface```
4. Auf der gleichen Seite, aktiviere die Checkbox ```AutoSaveRAM``` und stelle die zeit auf 90s
5. Wechsel aufs ``` -> General``` Tab
6. Aktiviere die Checkboxen ```Accept background input``` und ```Run in background```
7. Schließe das Fenster und gehe zu ```Config -> Hotkeys```, unten bei *Misc* wähle ```Clear All```

## Controller Konfigurieren

- Um das Controller Menu zu laden, muss eine Rom laufen
- Zu finden bei ```Config -> Controller```
- Selbst einstellen


## Video konfigurieren

- Da Multiworld ganz schön Leistung zieht, sollte man noch was anpassen
- Bei ```Config -> Cores -> N64 Video Plugin Settings``` Auflösung runterstellen.

**Um alle Einstellungen dauerhaft zu speichern, gehe zu ```Config -> Save Config```**

## Session konfigurieren

1. Gehe zu ```Tools -> Lua Console``` -> *Dieses Fenster MUSS immer offen sein, damit die Multiworld verbindung steht*
2. Gehe in *Settings*, check ```Disable Scripts on loads```
3. Emulator neustarten

# Hamachi installieren
Da Vodafone absolut KERNBEHINDERT ist, kann niemand von uns host sein. Deswegen nutzen wir Hamachi, *like in the good'ole days*

1. auf [https://www.vpn.net/] gehen
2. Downloaden und installieren
3. Account erstellen wenn gefragt


## Session starten

1. Hamachi öffnen
2. Zum Netzwerk connecten: 25.80.193.232, Name: CDootMultiRand PW: cdoot1234
3. Emulator öffnen
4. Rom laden
5. Lua Konsole öffnen
6. Open Script, wähle ```bizhawk co-op.lua``` im *Bizhawk 2.3* Ordner
7. Neue zeile taucht auf, doppelklicken -> *Dieses Fenster MUSS auch immer offen sein*
8. Oben bei *Rooms* ```Custom IP``` auswählen
9. Im *Host-IP* Feld, die IP von Hamachi eintragen (25.80.193.232)
10. Selbst Username wählen. Das ist euer In Game Name bei anderen.
11. Bei *Player #* die letzte Zahl euerer Rom wählen, da wo P*x* steht, das *x*  
12. Bei *Game Script* OOT auswählen
13. Connect
14. Ready setzen
