# CAN Protocol - LNCP -LabNet CAN Protokoll

## Eckdaten

CAN extended IDs - 29 Bit  
3 Bit Telegram Klassifizierung  
9 Bit HW Adresse (512)
9 Bit SW Adresse (512)
9 Bit Funktions Adresse (512 Funktionen/Register)

## Maskierung

Klassifizierung | HW ID | SW ID | Funktion ID
------------- | ------------- | ------------- | -------------
xx | xx xxxx xxx | x xxxx xxxx | xxxx xxxx x

### Klassifizierung

* 2 Bit  
* Bit 0-1

### HW ID

* 9 Bit
* 512 IDs
* Bit 2-11

### SW ID

* 9 Bit
* 512 IDs
* Bit 12-20

### Node ID

Kombination aus HW und SW ID.

### Funktion ID / Register

* 9 Bit
* 512 IDs
* Bit 21-29

## Beispiele

* direktes Ansprechen eines HW Nodes
* HW ID 1 
* Register 2

Klassifizierung | HW ID | SW ID | Funktion ID
------------- | ------------- | ------------- | -------------
01 | 00 0000 001 | 0 0000 0000 | 0000 0001 0

* Sensor Broadcast 
* HW ID 1
* SW ID 2
* Sensor ID 4

Klassifizierung | HW ID | SW ID | Funktion ID
------------- | ------------- | ------------- | -------------
11 | 00 0000 001 | 0 0000 0010 | 0000 0010 0