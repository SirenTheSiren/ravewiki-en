Windows Updates mit PowerShell durchführen
=====

PSWindowsUpdate installieren
####

- ``Install-Module -Name PSWindowsUpdate``
- ``Import-Module -Name PSWindowsUpdate``

Gegebenenfalls die "Execution Policy" anpassen
####

- ``Get-ExecutionPolicy -List``
- ``Set-ExecutionPolicy -ExecutionPolicy AllSigned -Scope CurrentUser``

Updates anrufen und installieren
####

- ``Get-WindowsUpdate``
- ``Install-WindowsUpdate``

https://www.thomas-krampe.com/2022/03/windows-updates-mit-powershell-durchfuehren/
