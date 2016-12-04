# LNCP - Lokale Events

## Feste Aktor IDs

Register    | Funktion 		| LENGHT		| Kommentar
----------  | ------------ 	| -------------	| -------------
 0x00 0010  |  RESET    	| 5				| write "RESET" to reboot hardware
 0x00 0011  |  defaultI 	| 8 			| write "DEFAULTI" to reset internal EEPROM
 0x00 0012  |  defaultE 	| 8 			| write "DEFAULTE" to reset external EEPROM
 0x00 000F  | 				| 8 			| 
 0x00 0010  | 				| 8 			| 
 0x00 001F  | 				| 8 			| 
 0x00 0020  | 				| 8 			| 
 0x00 002F  | 				| 8 			| 
 0x00 0030  | Rittal1		| 8 			| rittel_u
 0x00 0031  | Rittal2		| 8 			| Byte 0: min Ampere
 0x00 0032  | Rittal3		| 8 			| Byte 1: max Ampere
 0x00 0033  | Rittal4		| 8 			| Byte 2-7: 0=AUS,1=AN,2=NO_CHANGE
 0x01 0000  | Clear Cards   | 5 			| write "CLEAR" to reboot hardware
 0x01 0001  | ADD/EDIT Card | 8				| 7 Byte ID + Settings
 0x01 0002  | REMOVE Card 	| 7				| 7 Byte ID
