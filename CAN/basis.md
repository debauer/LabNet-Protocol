# CAN Protocol - LNCP -LabNet CAN Protokoll

## Eckdaten

CAN extended IDs - 29 Bit  
3 Bit Telegram Klassifizierung  
9 Bit HW Adresse (512)
9 Bit SW Adresse (512)
9 Bit Funktions Adresse (512 Funktionen/Register)

## Maskierung

### Telegram Klassifizierung

| Klassifizierung | other | 
| xx | 00 0000 0000 0000 0000 0000 0000 000 |

#### K#00 - Service

#### K#01 - Event Broadcast

##### F#0 - F#0fff ffff f 

#### K#10 - Node direkt

#### K#00 - Sensor Broadcast