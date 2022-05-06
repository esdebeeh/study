# SQLMap - Automatic SQL injection and database takeover tool
>Attempts to automatically identify and exploit SQL injection when supplied with a target URL.
>If you were performing a web application pentest and identified a potential SQL injection in a form using Burp Scanner, you could take the URL and give it to SQLmap. SQLmap would attempt to identify a working SQL injection string so that you could exploit the vulnerability and examine the impact or provide a proof of concept for exploitation during the pentest.

##### Usage: `sqlmap -u "http:///cat.php?id=1"`
___
- MITRE: 
	[Reconnaissance](https://attack.mitre.org/tactics/TA0043/) -> [T1595 Active Scanning](https://attack.mitre.org/techniques/T1595/) -> [002 Vulnerability Scanning](https://attack.mitre.org/techniques/T1595/002/)
- Publisher / Developer: 
	- [Bernardo Damele Assumpcao Guimaraes](mailto:bernardo@sqlmap.org)
	- [Miroslav Stampar](mailto:miroslav@sqlmap.org).
- OS: #UnixLike 
- License: https://github.com/sqlmapproject/sqlmap/blob/master/LICENSE

##### Links:
- Website: https://sqlmap.org/
- Docs: https://github.com/sqlmapproject/sqlmap/wiki/Usage
- Github / Wikipedia: https://github.com/sqlmapproject/sqlmap
- TryHackMe: 
	- https://tryhackme.com/room/sqlmap
	- https://tryhackme.com/room/sqlibasics
	- https://tryhackme.com/room/sqlilab
	- https://tryhackme.com/room/revenge
	- https://tryhackme.com/room/dailybugle (Hard)
- HTBAcademy:
	- https://academy.hackthebox.com/module/details/58 - SQLMap Essentials
	- https://academy.hackthebox.com/module/details/110 - Using Web Proxies
	- https://academy.hackthebox.com/module/details/112 - Footprinting

## Screens:
![[sqlmap_screen_1.png]]
![[sqlmap_screen_2.png]]


