# Changing Permissions (Readability)

## My Solve:
The goal was to make the /flag file readable, as it was not readable by the current user initially. 
I used the chmod command to add the read permission (+r) to the file. 
Using cat afterward successfully read the file's content and retrieved the flag.

*Flag*: pwn.college{cSgiMSsucnox5rFQtfFjKn5tUFYP.QXzcJM1WCOwMzNzEzW}
 
Bash

'''hacker@permissions\~changing-permissions:~$ chmod +r /flag            
hacker@permissions\~changing-permissions:~$ cat /flag              
pwn.college{cSgiMSsucnox5rFQtfFjKn5tUFYP.QXzcJM1WCOwMzNzEzW}'''              

## Notes And Errors:
None.

## References:
None.







