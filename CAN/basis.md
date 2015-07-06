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

### Funktion ID / Register

* 9 Bit
* 512 IDs
* Bit 21-29
