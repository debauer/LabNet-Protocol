# LNCP - Sensoren, Zustände

## Feste Sensor IDs

Anfrage via Remote REQ

Register    | Funktion 		| LENGHT		 | Kommentar
----------  | ------------ 	| -------------  | -------------
 0x00 0000  | Temperatur1	| 6 			 | ASCII "000.00"
 0x00 000F  | Temperatur16	| 6 			 | 
 0x00 0010  | Voltage1		| 8 			 | ASCII "0000.000"
 0x00 001F  | Voltage16		| 8 			 | ASCII "0000.000"
 0x00 0020  | Fuses			| 8 			 | Byte 0-7: 0=undef,1=OK,2=Kaputt
 0x00 0030  | Rittal1		| 8 			 | rittal_u
 0x00 0031  | Rittal2		| 8 			 | 
 0x00 0032  | Rittal3		| 8 			 | 
 0x00 0033  | Rittal4		| 8				 | 
 0x00 0040  | 				|  				 | 				 