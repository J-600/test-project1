# test-project1

@echo off
set "software_path=C:\percorso\del\file_installer.exe"
echo Installazione in corso senza permessi di amministratore...
reg add HKCU\Software\Classes\exefile\shell\runas /d "runas" /f >nul
start "" "%software_path%"
exit