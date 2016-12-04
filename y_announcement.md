# LNCP - Sensoren, Zustände

## Feste Sensor IDs

Anfrage via Remote REQ // zyklisches versenden

### Adressen für den Lab Einsatz 

Register    | Funktion 		| LENGHT		 | Kommentar
----------  | ------------ 	| -------------  | -------------
 0x00 0000  | Temperatur1	| 6 			 | ASCII "000.00"
 0x00 000F  | Temperatur16	| 6 			 | ASCII "999.99"
 0x00 0010  | Voltage1		| 8 			 | ASCII "0000.000"
 0x00 001F  | Voltage16		| 8 			 | ASCII "9999.999"
 0x00 0020  | Fuses			| 8 			 | Byte 0-7: 0=undef,1=OK,2=Kaputt
 0x00 0030  | Rittal1		| 8 			 | rittal_u
 0x00 0031  | Rittal2		| 8 			 | Byte 0: min Ampere
 0x00 0032  | Rittal3		| 8 			 | Byte 1: max Ampere
 0x00 0033  | Rittal4		| 8				 | Byte 2-7: 0=AUS,1=AN,2=NO_CHANGE
 0x01 0000  | Card Status	| 8 			 | 2 Byte Karten Anzahl im Speicher
 0x01 0001  | Card Invalid	| 7 			 | 7 Byte ID 
 0x01 0002  | Card OK		| 7 			 | 7 Byte ID 
 0x01 0000  | Card Status	| 8 			 | 7 Byte ID + Settings

### Adressen für den KFZ Einsatz 


Register    | Funktion 		| LENGHT		 | Kommentar
----------  | ------------ 	| -------------  | ------
 0xAA 0000  | OBD Kühlwassertemperatur 				| 8 | 		
 0xAA 0001  | OBD Kraftstoffdruck 					| 8 |
 0xAA 0002  | OBD Absoluter Luftdruck im Einlaßkanal | 8 | 
 0xAA 0003  | OBD Motordrehzahl 					| 8 | 
 0xAA 0004  | OBD Fahrzeuggeschwindigkeit 			| 8 | 
 0xAA 0005  | OBD Zündwinkel, Zylinder 1 			| 8 | 
 0xAA 0006  | OBD Ansaugluft-Temperatur 			| 8 | 
 0xAA 0007  | OBD Luftdurchfluß 					| 8 | 
 0xAA 0008  | OBD Absolute Drosselklappen-Position 	| 8 | 
 0xAA 0009  | OBD Zeit seit Motorstart 				| 8 | 
 0xAA 000A  | OBD Kraftstoffdruck 					| 8 | 
 0xAA 000B  | OBD Fahrtstrecke seit Motorleuchte an ist | 8 | 
 0xAA 000C  | OBD Laufzeit des Motors seit Motorleuchte an ist  | 8 | 
 0xAA 000D  | OBD Tankfüllstand 					| 8 | 
 0xAA 000E  | OBD Barometrischer Umgebungsdruck 	| 8 | 
 0xAA 000F  | OBD Ambient air temperature 			| 8 | 
 0xAA 0010  | OBD Absolute Throttle Position B 		| 8 | 
 0xAA 0011  | OBD Absolute Throttle Position C 		| 8 | 
 0xAA 0012  | OBD Accelerator Pedal Position D 		| 8 | 
 0xAA 0013  | OBD Accelerator Pedal Position E 		| 8 | 
 0xAA 0014  | OBD Accelerator Pedal Position F 		| 8 | 
 0xAB 0000  | Wassertankfüllstand | 8 |
 0xAB 0001  | Tankfüllstand 1 | 8 |
 0xAB 0002  | Tankfüllstand 2 | 8 |
 0xAB 0003  |  | 8 |
 0xAB 0004  |  | 8 |
 0xAB 0005  |  | 8 |
 0xAB 0006  |  | 8 |
 0xAB 0007  |  | 8 |
 0xAB 0008  |  | 8 |
 0xAB 0009  |  | 8 |
 0xAB 000A  |  | 8 |
 0xAB 000B  |  | 8 |
 0xAB 000C  |  | 8 |
 0xAB 000D  |  | 8 |
 0xAB 000E  |  | 8 |
 0xAB 000F  |  | 8 |
 0xAB 0010  | Temperatur innen | 8 |
 0xAB 0011  | Temperatur außen | 8 |
 0xAB 0012  | Temperatur 3 | 8 |
 0xAB 0013  | Temperatur 4 | 8 |
 0xAB 0014  | Temperatur 5 | 8 |
 0xAB 001F  | Temperatur 16 | 8 |
