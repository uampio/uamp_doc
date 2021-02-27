---
description: Error codes
---

# Error codes

| Error | Definition | Comments / Examples |
| :--- | :--- | :--- |
| `0xE000_0000` | [No error](0xe000_0000-no-error.md) | There is no error in the system |
| `0xE1XX_XXXX` | [Field bus error \(CANBus, EtherCAT, Profinet, ...\)](0xe1xx_xxxx-field-bus-related-errors.md) | Message not valid, slave not responding, etc … |
| `0xE2XX_XXXX` | [Communication error \(OPC-UA, DDS, ...\)](0xe2xx_xxxx-communication-error-opc-ua-dds-....md) | Server not accessible, Authentication error, etc … |
| `0xE3XX_XXXX` | [Hardware related error](0xe3xx_xxxx-hardware-related-error.md) | Driver mosffets error, Overcurrent, PLC error, etc … |
| `0xE4XX_XXXX` | [Actuator related error \(Motor, Piston, ...\)](0xe4xx_xxxx-actuator-related-error.md) | Stuck motor, Home position not reached, etc … |
| `0xE5XX_XXXX` | [Sensor related error](0xe5xx_xxxx-sensor-related-error.md) | Sensor not responding, Dust in the window sensor \(Scanners\), etc … |
| `0xE6XX_XXXX` | [PackML state machine error](0xe6xx_xxxx-application-reserved.md) | Runout timer switching state |
| `0xE7XX_XXXX` | [Application reserved](0xe7xx_xxxx-application-reserved.md) | Slave machine type A didn’t end the cycle, Slave machine error, Not expected datamatrix, etc … |

{% hint style="info" %}
If no sub level errors are required. Fill with zero. For example if we want to indicate a general error in actuators: 0xE400\_0000 should be used.
{% endhint %}

{% hint style="danger" %}
Errors will trigger machine to stop
{% endhint %}

