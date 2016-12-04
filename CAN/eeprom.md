# LNCP - Node - EEPROM

## Eckdaten

Extern - Onboard @ Basis - Adresse 0: 
Schreib/lesbar via EEPROM Telegramme
32k EEPROM - 4096 Byte - 12Bit Adresse

Intern: 
1028bit - 128Byte EEPROM
Sind als 16 Register verfügbar

Extern - RFID Karten - Adresse 1: 

### Karten Speicher

7 Byte Karten ID + 1 Byte Setting - Passt in ein Telegram  
Bei 32Kbit eeprom passen 512 Karten in den Speicher.
Wenn Speicherplatz leer ist wird Karten ID genullt
