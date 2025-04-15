# d-link DIR-619L has  buffer overflow vulnerability  in formSetWAN_Wizard56



## Information

- Vendor:https://www.dlink.com/
- Firmware:https://www.dlinktw.com.tw/techsupport/download.ashx?file=3803
- Affected Version: 2.04B04



## Vulnerability Analysis

The program receives the value of the host field through the `websGetVar` function,concatenates it into a formatted string using the `sprintf` function. Since the `sprintf` lacks the boundary check and the attacker's input length isn't checked either , buffer overflow exists.

![image-20250414000030179](Buffer_overflow-.assets\image-20250414000030179.png)

## PoC

 Due to legal and policy reasons, we are unable to provide the exploit for this  vulnerability at this time.



##  Note

The vendor was contacted early about this disclosure but did not respond in any  way.

