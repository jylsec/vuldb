# tp-link WR743ND has  buffer overflow vulnerability  in sub_42DDC4



## Information

- Vendor:https://www.tp-link.com/
- Firmware:https://static.tp-link.com/resources/software/TL-WR743ND_V2_120727.zip
- Affected Version: 2.120727

## Vulnerability Analysis

The program receives the value of the host field through the `httpGetEnv` function, copy it using the `strncpy` function. Since the attacker's input length isn't checked either , buffer overflow exists.

![code](code.png)

## PoC

 Due to legal and policy reasons, we are unable to provide the exploit for this  vulnerability at this time.



##  Note

The vendor was contacted early about this disclosure but did not respond in any  way.

