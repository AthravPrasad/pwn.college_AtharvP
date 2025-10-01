# Exporting Variables

## My Solve:
I exported the variable PWN with the value COLLEGE using the export keyword. I then set a second variable COLLEGE to the value PWN without using export. 
Running /challenge/run confirmed that PWN was correctly available to the sub-process and gave the flag.

*Flag:* pwn.college{cV6HtQsjLC3R_sl90B3rpCfHK9a.QXyYTN0wCOwMzNzEzW}

Bash

hacker@variables\~exporting-variables:~$ export PWN=COLLEGE     
You've set the PWN variable to the proper value!           
hacker@variables\~exporting-variables:~$ COLLEGE=PWN         
You've set the PWN variable to the proper value!         
You've set the COLLEGE variable to the proper value!        
hacker@variables\~exporting-variables:~$ /challenge/run       
CORRECT!          
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great        
job! Here is your flag:        
pwn.college{cV6HtQsjLC3R_sl90B3rpCfHK9a.QXyYTN0wCOwMzNzEzW}       
You've set the PWN variable to the proper value!         
You've set the COLLEGE variable to the proper value!         


## Notes and Errors:
None.

## References:
None.












Tools

