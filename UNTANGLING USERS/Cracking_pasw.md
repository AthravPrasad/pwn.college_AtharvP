# Cracking Passwords with john


## My Solve:
I used the john (John the Ripper) tool to crack the password hashes provided in /challenge/shadow-leak. 
After the cracking process was complete, I ran john again with the --show option to display the recovered credentials. 
The password for the user zardus was found to be aardvark. 
Finally, I used the su zardus command along with the cracked password to switch users and execute /challenge/run to retrieve the flag.

*Flag:* pwn.college{0e9MGW-7Anf4c5To0CPmx_fmhdx.QX3UDN1wCOwMzNzEzW}

Bash

'''hacker@users\~cracking-passwords:~$ john /challenge/shadow-leak            
Created directory: /home/hacker/.john                       
Loaded 1 password hash (crypt, generic crypt(3) [?/64])          
Press 'q' or Ctrl-C to abort, almost any other key for status         
aardvark          (zardus)        
1g 0:00:00:22 100% 2/3 0.04470g/s 260.3p/s 260.3c/s 260.3C/s Johnson..buzz            
Use the "--show" option to display all of the cracked passwords reliably          
Session completed          
hacker@users\~cracking-passwords:~$ john /challenge/shadow-leak --show         
hacker:NO PASSWORD:20357:0:99999:7:::        
zardus:aardvark:20364:0:99999:7:::           
         
2 password hashes cracked, 0 left         
hacker@users\~cracking-passwords:~$ su zardus        
Password:        
zardus@users\~cracking-passwords:/home/hacker$ /challenge/run        
Congratulations, you have become Zardus! Here is your flag:          
pwn.college{0e9MGW-7Anf4c5To0CPmx_fmhdx.QX3UDN1wCOwMzNzEzW}'''          


## Notes and Errors: 
None.

## References:
None.
