# LNCP - Register

## Internal EEPROM  Register

Ins interne EEPROM passen 16 Register

Register 	| Funktion | Kommentar
---------- 	| ------------ | -------------
0x000   |  UUID  	| - 48Bit Unique ID eines DS18D20 
0x001   |  Name  	| 1. Part 8 Buchstaben ASCII
0x002   |  Name  	| 2. Part 8 Buchstaben ASCII
0x003   |  Uptime  	| "00001337" -> 1337 Sekunden - 190 Jahre sollten reichen
0x004   |  unused 	| 
0x005   |  unused 	| 
0x006   |  unused 	| 
0x007   |  unused 	| 
0x008   |  unused 	| 
0x009   |  unused 	| 
0x00A   |  unused 	| 
0x00B   |  unused 	| 
0x00C   |  unused 	| 
0x00D   |  unused 	| 
0x00E   |  unused 	| 
0x00F   |  unused 	| 

## Flüchtige Register

Register 	| Funktion | Kommentar
---------- 	| ------------ | -------------
0x013   |  Status  	| "error", "ok", "sleep", "warning"...
0x014   |  Uhrzeit  | "133712  " -> HourMinuteSeconds - "no clock" -> no clock
0x015   |  Datum  	| "19121988" -> DayMonthYear - "no clock" -> no clock