CVE logo
Submit a CVE Request
* Required
* Select a request type
Report Vulnerability/Request CVE ID
* Enter your e-mail address
jylsec@gmail.com
alert

alert
IMPORTANT: Please add cve-request@mitre.org and cve@mitre.org as safe senders in your email client before completing this form.

IMPORTANT: Once a CVE ID is assigned to your vulnerability, it will not be published in the CVE List until you have submitted a URL pointing to public information about the vulnerability. Without a public reference, the CVE ID will display as "RESERVED" in the CVE List. Please update CVE with a reference to the vulnerability's details as soon as possible. See this FAQ for more information.
Enter a PGP Key (to encrypt)
If you would like us to send an encrypted response, please provide a PGP key up to 20,000 characters. If your PGP key is longer than 20,000 characters, please provide a URL or contact us at cve@mitre.org to identify an alternative solution.
* Number of vulnerabilities reported or IDs requested (1-10) info 
3
 Do you need more than 10 IDs?
This page will automatically update to provide one request form for each of the CVE IDs requested.
alert
Before submitting this request you should check whether the affected vendor is a CNA (see https://www.cve.org/ProgramOrganization/CNAs). Vulnerabilities in CNA products must be sent to the vendor in question. Also you should confirm that the vulnerability does not already have a CVE ID (see https://www.cve.org/About/Process)

* I have verified that this vulnerability is not in a CNA-covered product. 
* I have verified that the vulnerability has not already been assigned a CVE ID. 
Request Form 1 of 3
Required
* Vulnerability type info 
Buffer Overflow
* Vendor of the product(s) info
TOTOLINK
Affected product(s)/code base info
* Product	* Version	
T6
V4.1.9cu.5241_B20210923
[-] Remove [+] Add

Optional
Has vendor confirmed or acknowledged the vulnerability? Yes No
Attack type info 
Remote
Impact info
Code Execution	Information Disclosure
Denial of Service	Other
Escalation of Privileges	
Affected component(s)
main function of cstecgi.cgi
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/1/README.md
Attack vector(s)
POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login&flag=ie8
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/1/README.md
Suggested description of the vulnerability for use in the CVE info
TOTOlink T6(V4.1.9cu.5241_B20210923) router has buffer overflow vulnerability.  Affected is the function main of the file cstecgi.cgi. POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login&flag=ie8 will leads to buffer overflow.
Discoverer(s)/Credits info
Jiayang Zhou
Reference(s) info
https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/1/README.md
http://totolink.net/
https://www.totolink.net/home/menu/detail/menu_listtpl/download/id/190/ids/36.html
Additional information
Please provide any additional information you want to share with us here.
Request Form 2 of 3
Required
* Vulnerability type info 
Buffer Overflow
* Vendor of the product(s) info
TOTOlLINK
Affected product(s)/code base info
* Product	* Version	
T6
V4.1.9cu.5241_B20210923
[-] Remove [+] Add

Optional
Has vendor confirmed or acknowledged the vulnerability? Yes No
Attack type info 
Remote
Impact info
Code Execution	Information Disclosure
Denial of Service	Other
Escalation of Privileges	
Affected component(s)
main function of cstecgi.cgi
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/2/README.md
Attack vector(s)
POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login&flag=1
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/2/README.md
Suggested description of the vulnerability for use in the CVE info
TOTOlink T6(V4.1.9cu.5241_B20210923) router has buffer overflow vulnerability.  Affected is the function main of the file cstecgi.cgi. POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login&flag=1 will leads to buffer overflow.
Discoverer(s)/Credits info
Jiayang Zhou
Reference(s) info
https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/2/README.md
http://totolink.net/
https://www.totolink.net/home/menu/detail/menu_listtpl/download/id/190/ids/36.html
Additional information
Please provide any additional information you want to share with us here.
Request Form 3 of 3
Required
* Vulnerability type info 
Buffer Overflow
* Vendor of the product(s) info
TOTOLINK
Affected product(s)/code base info
* Product	* Version	
T6
V4.1.9cu.5241_B20210923
[-] Remove [+] Add

Optional
Has vendor confirmed or acknowledged the vulnerability? Yes No
Attack type info 
Remote
Impact info
Code Execution	Information Disclosure
Denial of Service	Other
Escalation of Privileges	
Affected component(s)
main function of cstecgi.cgi
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/3/README.md
Attack vector(s)
POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login
detail can be seen in https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/2/README.md
Suggested description of the vulnerability for use in the CVE info
TOTOlink T6(V4.1.9cu.5241_B20210923) router has buffer overflow vulnerability.  Affected is the function main of the file cstecgi.cgi. POST an overly long BODY to http://ip/cgi-bin/cstecgi.cgi?action=login&flag=1 will leads to buffer overflow.
Discoverer(s)/Credits info
Jiayang Zhou
Reference(s) info
https://github.com/jylsec/vuldb/blob/main/TOTOLINK/T6/3/README.md
http://totolink.net/
https://www.totolink.net/home/menu/detail/menu_listtpl/download/id/190/ids/36.html
Additional information
Please provide any additional information you want to share with us here.
alertBy clicking the submit button, you are agreeing to the CVE Terms of Use.
Enter Security Code
Retype the CAPTCHA code from the image 
nd4ak

errors Some fields on the form are not complete or are invalid. Complete the highlighted fields in red.

- Please select a Vulnerability type
 
Legal
Terms of Use
Privacy Policy
Media
News
Events
Sign up for e-newsletter
Social Media
  
New CVE Records
 CVE Announce
Contact
CVE Program Support
CNA
CVE Website Support
Use of the CVE® List and the associated references from this website are subject to the terms of use. CVE is sponsored by the U.S. Department of Homeland Security (DHS) Cybersecurity and Infrastructure Security Agency (CISA). Copyright © 1999-2023, The MITRE Corporation. CVE and the CVE logo are registered trademarks of The MITRE Corporation.