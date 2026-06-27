## Web Installer

Mit diesem Tool kannst du das vollständige Backup des ESP32‑C3 Mini AI‑Sprachdialog Modul für Revisionv0.4 mit 16MB Flash zurückspielen.

Projektseite: [Prilchen LABS](https://prilchen.de/ai-sprachdialog-mit-einem-kleinen-esp32-c3/)

Amazon: [ESP32_c3 Modul Revisionv0.4](https://amzn.to/4aTyhv8)

Verwendung in eigener Verantwortung. 



<a href="https://deinname.github.io/dein-repo/webinstaller.html">
  <img src="https://img.shields.io/badge/Flash%20Firmware-ESP%20Web%20Tools-blue?logo=espressif" />
</a>

[ESP Web Installer starten](https://prilchen.github.io/ESP32-C3MiniAI-Sprachdialogwebinstaller/)

INFO:

Details zum ESP32 und wie Image erstellt wurde

<img width="1053" height="382" alt="cmd1" src="https://github.com/user-attachments/assets/77de3c20-ecf4-4589-ae93-5e543af6f7e9" />

Alternativ manuell mit dem ESPTool zurück spielen:

Im Gerätemanager COM Port suchen und bei COMX eintragen Beispiel COM 10 = COM10
Prüfen ob Modul identisch ist mit 
python -m esptool -p COMX chip_id

Mudul löschen:
python -m esptool -p COMX erase_flash

Image downloaden und mit aufspielen
python -m esptool -p COMX write_flash 0x00000 esp32_c3_ki_r04_backup.bin

