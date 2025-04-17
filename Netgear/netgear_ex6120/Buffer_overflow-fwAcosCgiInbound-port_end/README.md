# Netgear EX6120 has  buffer overflow vulnerability  in fwAcosCgiInbound



## Information

- Vendor:https://www.netgear.com/
- Firmware:https://www.downloads.netgear.com/files/GDC/EX6120/EX6120-V1.0.0.68_1.0.41.zip?_ga=2.262151055.2092640780.1744442456-1939626221.1744442455
- Affected Version: 1.0.0.68





## Vulnerability Analysis

The program receives the value of the host field through the `websGetVar` function,copy it using the `strcpy` function. Since the `strcpy` lacks the boundary check and the attacker's input length isn't checked either , buffer overflow exists.

![code1](code1.png)

![code2](code2.png)

![code3](code3.png)

## PoC

 Due to legal and policy reasons, we are unable to provide the exploit for this  vulnerability at this time.



##  Note

The vendor was contacted early about this disclosure but did not respond in any  way.

