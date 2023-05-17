# NANDandNORgates
Designing 2-input CMOS NAND and NOR gates with open source EDA tool (Electric) and using LTSpice to observe the output


Code for the NOR gate
.INCLUDE C5_models.txt
.PARAM SUPPLY = 5
VDD VDD 0 DC 'SUPPLY'
Va A 0 pulse 0 'SUPPLY' 0 1n 1n 5n 10n
Vb B 0 pulse 0 'SUPPLY' 0 1n 1n 10n 15n
.TRAN 300n

Code for the NAND gate
.INCLUDE C5_models.txt
.PARAM SUPPLY = 5
.TRAN 300n
VDD VDD 0 DC 'SUPPLY'
Va A 0 pulse 0 'SUPPLY' 0 1n 1n 5n 10n
Vb B 0 pulse 0 'SUPPLY' 0 1n 1n 10n 15n
