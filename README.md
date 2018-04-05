# vnote

** Hello world
SD
ED
FD
Frequency

Frequency List:
SD Year + FD till ED + FD

Map<Date, Type> TLs
put(SD, 0)
put(ED, 3)
put(Frequency List.filter(d -> d > SD && d < ED), 1)

Sinker List:
put(Frequency List.filter(d -> d > SD && d < ED), 2)
sum(SAmount)

sort(TLs)

double Amount=CAmount||sum(SAmount)

Type 0: Amount=Amount Principal=0 Frequency=0 Interest=0
Type 1: Amount=Amount Principal=0 Frequency=Days||Frequency formula Interest=(Principal + Amount) * Coupon / Frequency
Type 2: Amount=Amount-SAmount Principal=SAmount Frequency=Days||Frequency formula Interest=(Principal + Amount) * Coupon / Frequency
Type 3: Amount=0 Principal=Amount Frequency=Days||Frequency formula Interest=(Principal + Amount) * Coupon / Frequency
