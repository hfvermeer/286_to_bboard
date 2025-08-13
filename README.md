# 286 to breadboard adapter
60-pin breadboard adapter for the 286 processor in PLCC-68 package

## Features
This slim design breadboard adapter for the 286 processor features the essential connections, descriptions, decoupling capacitors and even a small array of debugging leds for the system pin outputs. 

The debugging leds are optional, and may be left unpopulated if desired. The debugging leds may be switched off too by cutting the solder jumper 'JP1', or re-enabled again by soldering the bridge. It is enabled by default.

The adapter may also use J3 to provide power pins on the bottom side that directly connect to the breadboard power lines.

## Hardware Documentation

### Connections

#### J1 - Breadboard Jumper Header 1

Pin | Description
--- | -----------
1   | HLDA
2   | <ins>PEACK</ins>
3   | COD/<ins>INT</ins>
4   | <ins>Lock</ins>
5   | M//<ins>IO</ins>
6   | <ins>BHE</ins>
7   | <ins>S1</ins>
8   | <ins>S0</ins>
9   | D15
10  | D14
11  | D13
12  | D12
13  | D11
14  | D10
15  | D9
16  | D8
17  | D7
18  | D6
19  | D5
20  | D4
21  | D3
22  | D2
23  | D1
24  | D0
25  | <ins>ERROR</ins>
26  | <ins>BUSY</ins>
27  | CLK
28  | RESET
29  | GND
30  | VCC

#### J2 - Breadboard Jumper Header 2

Pin | Description
--- | -----------
1   | HOLD
2   | PEREQ
3   | NMI
4   | INTR
5   | <ins>READY</ins>
6   | GND
7   | A23
8   | A22
9   | A21
10   | A20
11  | A19
12  | A18
13  | A17
14  | A16
15  | A15
16  | A14
17  | A13
18  | A12
19  | A11
20  | A10
21  | A9
22  | A8
23  | A7
24  | A6
25  | A5
26  | A4
27  | A3
28  | A2
29  | A1
30  | A0

#### J3 - Breadboard Jumper Header 3 (Optional)

Pin | Description
--- | -----------
1   | VCC
2   | GND

### Bill of Materials (BOM)

Component type | Reference | Description | Quantity | Source and notes
-------------- | --------- | ----------- | -------- | ----------------
Capacitor | C1, C3, C4, C5 | 100nf, 0805 | 4 | 
Capacitor | C2 | 10uf, 0805 | 1 | 
Capacitor | C6 | 47nf, 0805 | 1 |
Capacitor | C7 | 100nf, 0402 | 1 | 
LED | D1, D2. D3, D4, D5, D6, D7, D8 | RED, 0603 | 8 |
Resistor | R1, R2. R3, R4, R5, R6, R7, R8 | 2k, 0402 | 8 |
Resistor | R9 | 1k, 0402 | 1 | 
Jumper | J1, J2 | Vertical, 2.54mm, SMT, pin1 left | 2 | 
Jumper | J3 | Vertical, 2.54mm, THT | 1 | 
IC | U1 | 74HC244, TSSOP-20 | 1 | 
Socket | UA1 | PLCC-68, SMT | 1 |

### Build Instructions

Hand solder under soldering microscope. The pads for connectors J1 and J2 contain via-in-pads. If using a stencil, these must be filled with tin prior to applying paste, otherwise they may wich up solder paste that is applied.

## Release Notes

### Changes

* Version 

* Version 1.0.0
  * Add component Values
  * Correct 74HC240 to 74HC244 in schematic
  * Correct label descriptions for GND, CLK, VCC and RESET
  * Add anchor plate for pin headers
  * Add Gerbers

* Version 0.9.0
  * Initial Release