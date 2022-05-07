# Nikto - Web Vulnerability Scanner
A free software command-line vulnerability scanner that scans webservers for dangerous files/CGIs, outdated server software and other problems. It performs generic and server type specific checks. It also captures and prints any cookies received.
-> <span style="color:red">Generates a lot of traffic, not a stealthy tool</span>

> A web server vulnerability scanner that tests for known vulnerabilities against target web URLs you provide. An example of using Nikto was given in Chapter 11, but you would use it to find known vulnerabilities pertaining to outdated plugin versions or other web software in cases where stealth is not a concern.

##### Usage: `perl nikto.pl -h target_ip -p target_port`
___
- MITRE: 
	- [Reconnaissance](https://attack.mitre.org/tactics/TA0043/) -> [T1595 Active Scanning](https://attack.mitre.org/techniques/T1595/) -> [002 Vulnerability Scanning](https://attack.mitre.org/techniques/T1595/002/)
- Publisher / Developer: https://en.wikipedia.org/wiki/Chris_Sullo
- License: GNU GPL v2

##### Links:
- Website: https://cirt.net/Nikto2
- Github: https://github.com/sullo/nikto
- Docs: https://github.com/sullo/nikto/wiki
- Wikipedia.org: https://en.wikipedia.org/wiki/Nikto_(vulnerability_scanner)
- TryHackMe: 
- HTBAcademy:
