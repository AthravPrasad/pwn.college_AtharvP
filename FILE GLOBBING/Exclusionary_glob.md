# Exclusionary Globbing
## My Solve:
The challenge required using an exclusionary bracket glob ([^...]) to match all files that do not start with the letters 'p', 'w', or 'n'. 
I used the pattern [^pwn]*, successfully returning the flag.

*Flag:* pwn.college{I3zhYflcd4cwjiJKwodmF8GkXka.QX2IDO0wCOwMzNzEzW}

Bash

hacker@globbing\~exclusionary-globbing:\~$ cd /challenge/files                           
hacker@globbing\~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]*          
You got it! Here is your flag!         
pwn.college{I3zhYflcd4cwjiJKwodmF8GkXka.QX2IDO0wCOwMzNzEzW}      
hacker@globbing\~exclusionary-globbing:/challenge/files$ 

## Notes and Errors:          
None.        

## References:
None.
