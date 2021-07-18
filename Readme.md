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

## Session konfigurieren

1. Gehe zu ```Tools -> Lua Console``` -> *Dieses Fenster MUSS immer offen sein, damit die Multiworld verbindung steht*
2. Gehe in *Settings*, check ```Disable Scripts on loads```
3. Um alle Einstellungen dauerhaft zu speichern, gehe zu ```Config -> Save Config```
4. Emulator neustarten

## Session starten

1. Lua Console öffnen
2. Open Script, wähle ```bizhawk co-op.lua``` im *Bizhawk 2.3* Ordner
3. Ein Rotes Quadrat wird in der Konsole auftauchen, doppelklicken -> *Dieses Fenster MUSS auch immer offen sein*
4. Im neuen Fenster folgendes angeben:
- Port: 50000
- *PW und Raum Folgen* 


