 ANLEITUNG
===========
1. Ordner erstellen
2. Ordner öffnen
3. SHIFT + Rechtsklick in den Ordner
4. Powershell Fenster hier öffnen
5. Script unten kopieren
6. Einfürgen in Powershell (Macht man einfach mit einem rechtsklick)
7. Warten, wenn Windows nach berechtigung fragt, akzeptieren.
8. Installer startet, installation durchführen.
- Done -

Script:

Set-ExecutionPolicy Bypass -Scope Process -Force;
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;
iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/TestRunnerSRL/bizhawk-co-op/master/bizhawk-co-op.ps1'))
