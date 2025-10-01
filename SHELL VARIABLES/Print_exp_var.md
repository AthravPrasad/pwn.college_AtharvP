# Printing Exported Variables

## My Solve:
I printed the list of all exported environment variables using the env command. The variable FLAG was visible in the output, containing the required flag.

*Flag:* pwn.college{UJycFSat0wb1lMS0BHrQMbgOjBW.QX4UTN0wCOwMzNzEzW}

Bash

hacker@variables\~printing-exported-variables:~$ env  
SHELL=/run/dojo/bin/bash        
HOSTNAME=variables~printing-exported-variables         
PWD=/home/hacker                
MANPATH=/run/dojo/share/man:       
DOJO_AUTH_TOKEN=ffe38c58035eef744b3c8271deb49b3422cef86e31333c6ba4e09b938ddfef88       
HOME=/home/hacker    
LANG=C.UTF-8       
FLAG=pwn.college{UJycFSat0wb1lMS0BHrQMbgOjBW.QX4UTN0wCOwMzNzEzW}    
TERMINFO=/run/dojo/share/terminfo           
TERM=xterm-256color            
SHLVL=2            
LC_CTYPE=C.UTF-8         
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt         
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin             
DEBIAN_FRONTEND=noninteractive                      
_=/run/dojo/bin/env   

## Notes and Errors:
None.

## References:
None.
