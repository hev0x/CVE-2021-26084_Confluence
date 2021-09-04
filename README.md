# CVE-2021-26084 - Confluence Server Webwork OGNL injection

- An OGNL injection vulnerability exists that would allow an authenticated user, and in some instances unauthenticated user, to execute arbitrary code on a Confluence Server or Data Center instance. 


### IMPORTANT
This exploit is only intended to facilitate demonstrations of the vulnerability by researchers. I disapprove of illegal actions and take no responsibility for any malicious use of this script. The proof of concept demonstrated in this repository does not expose any hosts and was performed with permission.


#### • queryString param Request
![]()![BurpRequest](https://user-images.githubusercontent.com/6265911/131630570-857df5dd-525d-43ec-9466-5c92ac9c1322.png)


### Exploit Usage

#### Commands:
`$ python3 Confluence_OGNLInjection.py -u http://xxxxx.com `

#### or
`$ python3 Confluence_OGNLInjection.py -u http://xxxxx.com -p /pages/createpage-entervariables.action?SpaceKey=x `



#### • Exploitation with Confluence_OGNLInjection.py
![Exploit](https://user-images.githubusercontent.com/6265911/131630805-147628fc-7772-47be-943e-12d24b052adb.png)



- References:

https://confluence.atlassian.com/doc/confluence-security-advisory-2021-08-25-1077906215.html
 
https://github.com/httpvoid/writeups/blob/main/Confluence-RCE.md

https://www.exploit-db.com/exploits/50243
