# Setting The PATH Variable

## My Solve:
The objective of this challenge was to ensure the /challenge/run program could find and execute a command named win located in a specific directory (/challenge/more_commands/). 
This required modifying the PATH environment variable.
I set the PATH environment variable to the directory containing the necessary executable: PATH=/challenge/more_commands/.
When the main program (/challenge/run) executed, it looked in the newly defined PATH location, successfully found and executed the win command, and printed the flag.

*Flag:*  pwn.college{cV7LBZTg6Dc6dDnvDcqnEWhmYJt.QX1cjM1wCOwMzNzEzW}

Bash

'''hacker@path\~setting-path:\~$ PATH=/challenge/more_commands/         
hacker@path\~setting-path:\~$ /challenge/run           
Invoking 'win'....         
Congratulations! You properly set the flag and 'win' has launched!            
pwn.college{cV7LBZTg6Dc6dDnvDcqnEWhmYJt.QX1cjM1wCOwMzNzEzW}'''              

## Notes And Errors:
None.

## References:
None.







