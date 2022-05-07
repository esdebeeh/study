# JTR: John The Ripper
>An offline password cracking tool. For CPU-based cracking, JtR is one of the fastest tools for password recovery. So, if GPU cracking is unavailable, you would use JtR. However, JtR also implements different rule sets than other cracking tools, and these rule sets may recover passwords where other cracking tools fail, so it is a good supplement to other cracking tools for large password lists.

#### Usage: `john --wordlist=<PATH_TO_WORDLIST> <HASHFILE>`
- MITRE:
	- [Credential Access]() -> [T1110 Brute Force](https://attack.mitre.org/techniques/T1110/) ->[002 Password Cracking](https://attack.mitre.org/techniques/T1110/002/)
- Publisher / Developer: OpenWall
- License: https://github.com/openwall/john-packages/blob/master/LICENSE.txt

#### Links:
- Website: https://www.openwall.com/john/
	- JTR Examples: https://www.openwall.com/john/doc/EXAMPLES.shtml
- Docs: https://github.com/openwall/john-packages/blob/master/readme.md
- Github / Wikipedia:
	- https://github.com/openwall/john-packages
	- https://en.wikipedia.org/wiki/John_the_Ripper
- TryHackMe: 
	- https://tryhackme.com/room/johntheripper0
- HTBAcademy: 
	- https://academy.hackthebox.com/module/details/147 - Password Attacks

##### cracking shadow hash:

/etc/passwd line
`root:x:0:0:root:/root:/bin/bash `

/etc/shadow line `root:$6$riekpK4m$uBdaAyK0j9WfMzvcSKYVfyEHGtBfnfpiVbYbzbVmfbneEbo0wSijW1GQussvJSk8X1M56kzgGj8f7DFN1h4dy1:18226:0:99999:7:::`

`$ unshadow passwd.txt shadow.txt > unshadowed.txt `

unshadowed.txt `root:$6$riekpK4m$uBdaAyK0j9WfMzvcSKYVfyEHGtBfnfpiVbYbzbVmfbneEbo0wSijW1GQussvJSk8X1M56kzgGj8f7DFN1h4dy1:0:0:root:/root:/bin/bash`
`$ john --wordlist=/usr/share/wordlists/rockyou.txt unshadowed.txt`
`$ zip2john protected.zip > zip.hashes `
`$ john --wordlist=/usr/share/wordlists/crypton.txt zip.hashes`

