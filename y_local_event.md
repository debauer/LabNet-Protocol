# LNCP - Lokale Events

## Feste Aktor IDs

Register    | Funktion 		| LENGHT		| Kommentar
----------  | ------------ 	| -------------	| -------------
 0x010  |  RESET    	| 5				| write "RESET" to reboot hardware
 0x011  |  defaultI 	| 8 			| write "DEFAULTI" to reset internal EEPROM
 0x012  |  defaultE 	| 8 			| write "DEFAULTE" to reset external EEPROM
 0x00F  | 				| 8 			| 
 0x010  | 				| 8 			| 
 0x01F  | 				| 8 			| 
 0x020  | 				| 8 			| 
 0x02F  | 				| 8 			| 
 0x031  | Rittal1		| 8 			| rittel_u
 0x032  | Rittal2		| 8 			| Byte 0: min Ampere
 0x033  | Rittal3		| 8 			| Byte 1: max Ampere
 0x034  | Rittal4		| 8 			| Byte 2-7: 0=AUS,1=AN,2=NO_CHANGE
 0x100  | Clear Cards   | 5 			| write "CLEAR" to delete all cards
 0x101  | ADD/EDIT Card | 8				| 7 Byte ID + Settings
 0x102  | REMOVE Card 	| 7				| 7 Byte ID
