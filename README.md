# Adobe Coldfusion BlazeDS Java Object Deserialization RCE

Exploit-DB: https://www.exploit-db.com/exploits/43993/

Exploit Title: Adobe Coldfusion BlazeDS Java Object Deserialization RCE

Date: February 6, 2018

Exploit Author: Faisal Tameesh (@DreadSystems)

Company: Depth Security (https://depthsecurity.com)

Version: Adobe Coldfusion (11.0.03.292866)

Tested On: Windows 10 Enterprise (10.0.15063)

CVE: CVE-2017-3066

Advisory: https://helpx.adobe.com/security/products/coldfusion/apsb17-14.html

Category: remote

Notes:
This is a two-stage deserialization exploit. The code below is the first stage.
You will need a JRMPListener (ysoserial) listening at callback_IP:callback_port.
After firing this exploit, and once the target server connects back, 
JRMPListener will deliver the secondary payload for RCE.
