# AHCA

## AHCA Simulation Cases

| **Temperature** | **Mode** | **Traffic Load \(%\)** | **PAR \(dB\)** |
| :--- | :--- | :--- | :--- |
| 45°C | 4x40W | 70 | 6.7 |
| 45°C | 4x40W | 70 | 8.1 |
| 30°C | 4x40W | 100 | 8.1 |
| 45°C | 2x60W | 70 | 6.7 |
| 30°C | 2x60W | 100 | 6.7 |

## X21 therml testing result

#### Overall

| 4\*30W, 3m/s effect | 18.6 |
| :--- | :--- |
| 2\*40W,3m/s effect | 17.7 |
| 4\*30W,0,5m/s effect | 9 |
| 2\*40W,0,5m/s effect | 5.3 |
| Chamber effect 4\*40W | 13.9 |
| Chamber effect 4\*30W | 10.8 |

#### PA

* Ta 22 to 45°C, +21.4°C. 1.6°C lower.
* 40°C, 45°C, 55°C device temperature linearly increase with Ta.
* 3m/s wind, -15°C.
* 100% to 70%, -6.9°C.
* 0.5m/s, solar, -2.2°C.
* 100% to 70% 0.5m/s, solar, -9°C.

#### TRX

* Ta 22 to 45°C, +21°C. 2°C lower.
* 40°C, 45°C, 55°C device temperature linearly increase with Ta.
* 


Goal:

* PA main flange 125°C
* PA heat sink 105°C
* PA temp sensor temperature 105°C
* TRX PWB 87°C

## RF performance testing

In hot temperature testing the temperature chamber was adjusted so that following PA temperatures were reachable:

| PA1 | PA2 | PA3 | PA4 | LNA1 | LNA2 | TRX1 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 95.6 | 97.7 | 98.5 | 94.4 | 84 | 86 | 81 |

## AHEGA & AHPMDA Thermal Test Plan

| **Case** | **Max. Amb.  \(°C\)** | **Traffic loading** | **Wind \(m/s\)** | **Solar Load** | **Covers** | **Criteria** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 6 | 25 | 50% load from nominal TX power with maximum crest factor | 3 m/s | None | None | MTBF |
| 7 | 40 | 70% load from nominal TX power with maximum crest factor | 0 | None | None | Specified Max |
| 8 | 55 | 50% load from nominal TX power with maximum crest factor | 0 | None | None | Specified Max |



> Due to pressures from Product Management to reduce the size and weight of the units, the Galaxy program and technical management have replaced some of the test cases in the guidelines with others that are more in line with the program's goals.

### TCS Point

| Amb Temp.  \[C\] | Traffic Conditions Description | RF Output Power \[% of Rated\] | Wind \[m/s\] | Input Voltage  \[VDC\] | Return Loss | Criteria | Comments |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 40 | 70% load from nominal Tx power with maximum crest factor | 70 | 0 | 60 | -30 dB | Specified Max | Used to determine DPC Start set point |
| 55 | 50% load from nominal Tx power with maximum crest factor | 50 | 0 | 60 | -30 dB | Specified Max | Used to determineT-protect |
| 50 | 50% load from nominal Tx power with maximum crest factor | 50 | 0 | 60 | -30 dB | - - - | Used to determineT-high and DPC End set point |
| 60 | 35% load from nominal Tx power with maximum crest factor | 35 | 0 | 60 | -30 dB | - - - | Used to determineT-danger |



