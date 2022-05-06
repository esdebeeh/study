## Brakeman - Ruby On Rails SAST Scanner
A free vulnerability scanner specifically designed for Ruby on Rails applications. It statically analyzes Rails application code to find security issues at any stage of development.
-> Brakeman looks at the source code of an application
-> Brakeman requires zero setup  or configuration

>If you need to perform static application security testing #SAST against a Ruby on Rails application, Brakeman will take Rails source code, scan it, and produce a report of potential security issues. 
>As with all automated code analysis tools, it may generate false positives, so its results should be manually reviewed. It will also miss issues that are introduced during runtime by interaction with other components, so it should be used with other tools and #DAST methodologies to fully evaluate an application for pentesting. It is run from the command line using dashed options (-A, -n, etc.) to define its behavior and can either target a specific application and path or run against the application in the current directory

##### Usage: `brakeman your_rails_app`
___
- MITRE: 
	- [Reconnaissance](https://attack.mitre.org/tactics/TA0043/) -> [T1595 Active Scanning](https://attack.mitre.org/techniques/T1595/) -> [002 Vulnerability Scanning](https://attack.mitre.org/techniques/T1595/002/)
- Publisher / Developer: Justin Collins aka https://presidentbeef.com/ns/
- OS: #UnixLike
- License: https://github.com/presidentbeef/brakeman/blob/main/LICENSE.md

##### Links:
- Website:  https://brakemanscanner.org/
- Docs: https://brakemanscanner.org/docs/
- Github: https://github.com/presidentbeef/brakeman
- TryHackMe: 
- HTBAcademy:
___
### Screens:
![[brakeman_screen_1.png]]
*Brakeman Static Code Analysis Output*

##### Confidence: 
This rating is intended to indicate how certain Brakeman is that the given warning is a real problem.
- <span style="color:red">High</span> - Either this is a simple warning or user input is very likely being used in unsafe ways.
- <span style="color:yellow">Medium</span> - This generally indicates an unsafe use of a variable, but the variable may or may not be user input.
- <span style="color:Green">High</span> - Typically means user input was indirectly used in a potentially unsafe manner.
___
### Reads:
- [[CompTIA_PT0-002_All-in-One_Guide.pdf]] - Page 571
- [[CompTIA_PT0-002_Sybex_Study_Guide.pdf]] - Page 70
- [[CompTIA_PT0-002_For_Dummies.pdf]] - Page 358