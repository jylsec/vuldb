# d-link DIR-605L has  command injection vulnerability  in wake_on_lan



## Information

- Vendor: https://www.dlink.com/
- Firmware: https://www.dlinktw.com.tw/techsupport/download.ashx?file=11582
- Affected Version: 2.13B01



## Vulnerability Analysis

The program receives the value of the host field through the `websGetVar` function,concatenates it into a formatted string using the `sprintf` function, and finally executes a system command using the `system` function. Since the attacker's inputis not filtered, any command can be executed.

![QQ截图20250412151844](Command_injection-wake_on_lan-mac.assets\QQ截图20250412151844.jpg)

## PoC

 Due to legal and policy reasons, we are unable to provide the exploit for this  vulnerability at this time.



##  Note

The vendor was contacted early about this disclosure but did not respond in any  way.

