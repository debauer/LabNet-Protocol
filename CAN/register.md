# LNCP - Register

## Default Register
Register | Funktion | Kommentar
---------- | ------------ | -------------
0   |  UUID  	| - 48Bit Unique ID eines DS18D20 + wenn SW Node wird die SW ID angehängt 
1   |  Name  	| 1. Part 8 Buchstaben ASCII
2   |  Name  	| 2. Part 8 Buchstaben ASCII
3   |  Typ  	| "Hardware", "Temp    ", "Moisture", "LCD", "7Segment"...
4   |  Status  	| "error", "ok", "sleep", "warning"...
5   |  Uptime  	| "00001337" -> 1337 Sekunden - 190 Jahre sollten reichen
6   |  Uhrzeit  | "133712  " -> HourMinuteSeconds - "no clock" -> no clock
7   |  Datum  	| "19121988" -> DayMonthYear - "no clock" -> no clock
8   |  RESET    | write "RESET   " to reboot hardware
9   |  unused 	| 
10  |  unused 	| 
11  |  unused 	| 
12  |  unused 	| 
13  |  unused 	| 
14  |  unused 	| 
15  |  unused 	| 
16  |  unused 	| 
17  |  unused 	| 
18  |  unused 	| 
19  |  unused 	| 
20  |  unused 	| 
21  |  unused 	| 
22  |  unused 	| 
23  |  unused 	| 
24  |  unused 	| 
25  |  unused 	| 
26  |  unused 	| 
27  |  unused 	| 
28  |  unused 	| 
29  |  unused 	| 
30  |  unused 	| 
31  |  unused 	| 
