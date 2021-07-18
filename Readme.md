# ANLEITUNG

## Emulator installieren

1. Ordner erstellen
2. Ordner öffnen
3. SHIFT + Rechtsklick in den Ordner
4. Powershell Fenster hier öffnen
5. Script unten kopieren
6. Einfügen in Powershell (Macht man einfach mit einem rechtsklick)
7. Warten, wenn Windows nach berechtigung fragt, akzeptieren.
8. Installer startet, installation durchführen.
9.  Im Ordner wurde alles erstellt, kann jetzt verschoben werden.


*Bei Problemen während der Installation, bitte bei Ihrem örtlichen Hannes melden.*


  **Done**

###### Script:
```
Set-ExecutionPolicy Bypass -Scope Process -Force;
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;
iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/TestRunnerSRL/bizhawk-co-op/master/bizhawk-co-op.ps1'))
```

## Emulator konfigurieren

1. Gehe zu ```Config -> Customize -> Advance```
2. 
