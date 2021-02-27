---
description: Information and communications codes
---

# Information codes



| Info | Definition | Comments / Examples |
| :--- | :--- | :--- |
| `0xC000_0000` | No information / communicate | There is no information message in the system |
| `0xC1XX_XXXX` | Field bus information \(CANBus, EtherCAT, Profinet, ...\) | Message not valid, slave not responding, etc … |
| `0xC2XX_XXXX` | Communication information \(OPC-UA, DDS, ...\) | Server not accessible, Authentication error, etc … |
| `0xC3XX_XXXX` | Hardware related information | Driver mosffets error, Overcurrent, PLC error, etc … |
| `0xC4XX_XXXX` | Actuator related information \(Motor, Piston, ...\) | Stuck motor, Home position not reached, etc … |
| `0xC5XX_XXXX` | Sensor related information | Sensor not responding, Dust in the window sensor \(Scanners\), etc … |
| `0xC6XX_XXXX` | PackML state machine information | Runout timer switching state |
| `0xC7XX_XXXX` | Application reserved information | Slave machine type A didn’t end the cycle, Slave machine error, Not expected datamatrix, etc … |

