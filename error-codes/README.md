---
description: Error codes
---

# Error codes

| Error | Definition | Comments / Examples |
| :--- | :--- | :--- |
| 0xE000\_0000 | No error | There is no error in the system |
| 0xE1XX\_XXXX | Field bus error \(CANBus, EtherCAT, Profinet, ...\) | Message not valid, slave not responding, etc … |
|  |  |  |

{% hint style="info" %}
If no sub level errors are required. Fill with zero. For example if we want to indicate a general error in actuators: 0x4000\_0000 should be used.
{% endhint %}

