# LNCP - Register

## Default Register

Ins interne EEPROM passen 16 Register

Register 	| Funktion | Kommentar
---------- 	| ------------ | -------------
0x00 0000   |  UUID  	| - 48Bit Unique ID eines DS18D20 
0x00 0001   |  Name  	| 1. Part 8 Buchstaben ASCII
0x00 0002   |  Name  	| 2. Part 8 Buchstaben ASCII
0x00 0003   |  Status  	| "error", "ok", "sleep", "warning"...
0x00 0004   |  Uptime  	| "00001337" -> 1337 Sekunden - 190 Jahre sollten reichen
0x00 0005   |  Uhrzeit  | "133712  " -> HourMinuteSeconds - "no clock" -> no clock
0x00 0006   |  Datum  	| "19121988" -> DayMonthYear - "no clock" -> no clock
0x00 0008   |  unused 	| 
0x00 0009   |  unused 	| 
0x00 000A   |  unused 	| 
0x00 000B   |  unused 	| 
0x00 000C   |  unused 	| 
0x00 000D   |  unused 	| 
0x00 000E   |  unused 	| 
0x00 000F   |  unused 	| 
0x00 0010   |  RESET    | write "RESET   " to reboot hardware
0x00 0011   |  defaultI | write "DEFAULT " to reset internal EEPROM
0x00 0011   |  defaultE | write "DEFAULT " to reset éxternal EEPROM