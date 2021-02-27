---
description: Error codes
---

# Error codes

| Error | Definition | Comments / Examples |
| :--- | :--- | :--- |
| [0xE000\_0000](0xe000_0000-no-error.md) | No error | There is no error in the system |
| [0xE1XX\_XXXX](0xe1xx_xxxx-field-bus-related-errors.md) | Field bus error \(CANBus, EtherCAT, Profinet, ...\) | Message not valid, slave not responding, etc … |
| [0xE2XX\_XXXX](0xe2xx_xxxx-communication-error-opc-ua-dds-....md) | Communication error \(OPC-UA, DDS, ...\) | Server not accessible, Authentication error, etc … |
| [0xE3XX\_XXXX](0xe3xx_xxxx-hardware-related-error.md) | Hardware related error | Driver mosffets error, Overcurrent, PLC error, etc … |
| [0xE4XX\_XXXX](0xe4xx_xxxx-actuator-related-error.md) | Actuator related error \(Motor, Piston, ...\) | Stuck motor, Home position not reached, etc … |
| [0xE5XX\_XXXX](0xe5xx_xxxx-sensor-related-error.md) | Sensor related error | Sensor not responding, Dust in the window sensor \(Scanners\), etc … |
| [0xE6XX\_XXXX](0xe6xx_xxxx-application-reserved.md) | PackML state machine error | Runout timer switching state |
| [0xE7XX\_XXXX](0xe7xx_xxxx-application-reserved.md) | Application reserved | Slave machine type A didn’t end the cycle, Slave machine error, Not expected datamatrix, etc … |

{% hint style="info" %}
If no sub level errors are required. Fill with zero. For example if we want to indicate a general error in actuators: 0xE400\_0000 should be used.
{% endhint %}

{% hint style="danger" %}
Errors will trigger machine to stop
{% endhint %}

