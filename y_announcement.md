# LNCP - Sensoren, Zustände

## Feste Sensor IDs

Anfrage via Remote REQ // zyklisches versenden

### Adressen für den Lab Einsatz 

Register    | Funktion 		| LENGHT		 | Kommentar
----------  | ------------ 	| -------------  | -------------
 0x000  | Temperatur1	| 6 			 | ASCII "000.00"
 0x00F  | Temperatur16	| 6 			 | ASCII "999.99"
 0x010  | Voltage1		| 8 			 | ASCII "0000.000"
 0x01F  | Voltage16		| 8 			 | ASCII "9999.999"
 0x020  | Fuses			| 8 			 | Byte 0-7: 0=undef,1=OK,2=Kaputt
 0x031  | Rittal1		| 8 			 | rittal_u
 0x032  | Rittal2		| 8 			 | 	Byte 0: min Ampere
 0x033  | Rittal3		| 8 			 | 	Byte 1: max Ampere
 0x034  | Rittal4		| 8				 | 	Byte 2-7: 0=AUS,1=AN,2=NO_CHANGE
 0x100  | Card Status	| 8 			 | 2 Byte Karten Anzahl im Speicher
 0x101  | Card Invalid	| 7 			 | 7 Byte ID 
 0x102  | Card OK		| 7 			 | 7 Byte ID 
 0x100  | Card Status	| 8 			 | 7 Byte ID + Settings

### Adressen für den KFZ Einsatz 


Register    | Funktion 		| LENGHT		 | Kommentar
----------  | ------------ 	| -------------  | ------
 0xA00  | OBD Kühlwassertemperatur 				| 8 | 		
 0xA01  | OBD Kraftstoffdruck 					| 8 |
 0xA02  | OBD Absoluter Luftdruck im Einlaßkanal | 8 | 
 0xA03  | OBD Motordrehzahl 					| 8 | 
 0xA04  | OBD Fahrzeuggeschwindigkeit 			| 8 | 
 0xA05  | OBD Zündwinkel, Zylinder 1 			| 8 | 
 0xA06  | OBD Ansaugluft-Temperatur 			| 8 | 
 0xA07  | OBD Luftdurchfluß 					| 8 | 
 0xA08  | OBD Absolute Drosselklappen-Position 	| 8 | 
 0xA09  | OBD Zeit seit Motorstart 				| 8 | 
 0xA0A  | OBD Kraftstoffdruck 					| 8 | 
 0xA0B  | OBD Fahrtstrecke seit Motorleuchte an ist | 8 | 
 0xA0C  | OBD Laufzeit des Motors seit Motorleuchte an ist  | 8 | 
 0xA0D  | OBD Tankfüllstand 					| 8 | 
 0xA0E  | OBD Barometrischer Umgebungsdruck 	| 8 | 
 0xA0F  | OBD Ambient air temperature 			| 8 | 
 0xA10  | OBD Absolute Throttle Position B 		| 8 | 
 0xA11  | OBD Absolute Throttle Position C 		| 8 | 
 0xA12  | OBD Accelerator Pedal Position D 		| 8 | 
 0xA13  | OBD Accelerator Pedal Position E 		| 8 | 
 0xA14  | OBD Accelerator Pedal Position F 		| 8 | 
 0xB00  | Wassertankfüllstand | 8 |
 0xB01  | Tankfüllstand 1 | 8 |
 0xB02  | Tankfüllstand 2 | 8 |
 0xB03  |  | 8 |
 0xB04  |  | 8 |
 0xB05  |  | 8 |
 0xB06  |  | 8 |
 0xB07  |  | 8 |
 0xB08  |  | 8 |
 0xB09  |  | 8 |
 0xB0A  |  | 8 |
 0xB0B  |  | 8 |
 0xB0C  |  | 8 |
 0xB0D  |  | 8 |
 0xB0E  |  | 8 |
 0xB0F  |  | 8 |
 0xB10  | Temperatur innen | 8 |
 0xB11  | Temperatur außen | 8 |
 0xB12  | Temperatur 3 | 8 |
 0xB13  | Temperatur 4 | 8 |
 0xB14  | Temperatur 5 | 8 |
 0xB1F  | Temperatur 16 | 8 |
