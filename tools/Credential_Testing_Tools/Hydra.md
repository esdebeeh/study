IMAGE / LOGO / ICON

# Hydra
>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum sed sollicitudin justo. Morbi efficitur congue nisi euismod fringilla. Suspendisse porta sed velit et lobortis.

##### Usage: `hydra <Target_IP> <Protocoll> -l <username> -P <password_file> -s <Port> -vV`
`-l: input login`
`-L: list of username`
`-p: single password
`-P: list of passwords`
##### brute force tfp username and password
`hydra -L <username_file> -P <password_file> ftp://<Target_IP>`
##### brute force telnet username and password
`hydra -l <username> -p <password> telnet://<Target_IP>`
##### brute force http post form
`hydra -l <USER> -p <PASSWORD> <IP_ADDRESS> http-post-form "<LOGIN_PAGE>:<REQUEST_BODY>:<ERROR_MESSAGE> PHPSESSID=<COOKIE>`
example
`hydra -l admin -p admin 10.10.15.42 http-post-form "/login:username=^USER^&pwd=^PASS^&submit=login:F=Invalid Credentials`
![[hydra.png]]
___
- MITRE:
- OS:
- License:

##### Links:
- Website: https://salsa.debian.org/pkg-security-team/hydra
- Docs: https://github.com/vanhauser-thc/thc-hydra/blob/master/README
- Github / Wikipedia: https://github.com/vanhauser-thc/thc-hydra
- TryHackMe: 
- HTB-Academy:

## Screens:

## Reads:
- Read 1 - https://www.kali.org/tools/hydra/