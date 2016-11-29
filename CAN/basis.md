# CAN Protocol - LNCP -LabNet CAN Protokoll

## Eckdaten

CAN extended IDs - 29 Bit  

5 Bit Telegram Typ
12 Bit NODE ID
12 Bit REGISTER

## Typen

### Broadcast Event 00000

0x00 Basis
0xXXXX XXXX XXXX Event ID


### Local Event 00001

0x01 Basis
0xXXXXXX Node ID
0xYYYYYY Event ID

Auf Node X Event Y ausführen mit Nutzdaten Z

### Register 00011

0x04 Basis
0xXXXXXX Node ID
0xYYYYYY Sensor

Register X auf Node Y mit 8 Byte Nutzdaten

### Announcement 00100

0x04 Basis
0xXXXXXX Node ID
0xYYYYYY Sensor

z.B. Sensordaten
Sensor X auf Node Y mit 8 Byte Nutzdaten

### Eeprom 01000 -> 01010

0x08 -> schreiben
0x09 -> anfragen
0x10 -> antwort

0x08 Basis
0xXXXXXX Node ID
0xYYYYYY eeprom Adresse (12Bit = 4096 byte = 32k eeprom)

Adresse = start Adresse im eeprom, von dort werden 1-8 Bytes ins eeprom geschrieben
Anfrage mit 1-8 Byte dummy daten für die Anzahl abzufragender Bytes.

### SF RXTX 01011

0x05 Basis
0xXXXXXX Node ID
0xYYYYYY SF

##### SF Seriel 0x000000 -> 0x0000FF

0x000000 Seriel Ziel (ASCII Ziel ID + console, seriel, rs485)
0x000001 Seriel Baud (ASCII Ziel ID + Baud 9600, 19200...)
0x000010 Seriel RX 1 
0x000011 Seriel RX 2 
...
0x00001F Seriel RX 8 
0x000010 Seriel TX Adr1 (an welchen Node soll TX gesendet werden)
0x000011 Seriel TX Adr2 (an welchen Node soll TX gesendet werden)
...
0x00001F Seriel TX Adr8 (an welchen Node soll TX gesendet werden)

Indem man 2 Nodes gegenseitig die TX adressen mitteilt kann man Seriell Tunneln und gleichzeitig den beiden zuhören. 

##### 
