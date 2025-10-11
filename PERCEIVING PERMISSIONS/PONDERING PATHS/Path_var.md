# The PATH Variable


## My Solve:
The objective was to prevent the /challenge/run program from executing the necessary utility to remove the flag file.
This relied on manipulating the PATH environment variable, which tells the shell where to look for executable commands.
I deliberately overwrote the PATH variable by setting it to an empty string with a single space: PATH=" ".
When /challenge/run subsequently attempted to execute the rm command (which is typically found in a directory listed in PATH), the shell could not locate the command, leading to an error (rm: command not found).
Because the flag removal failed, the program printed the flag directly as a failure state.

*Flag:* pwn.college{s0QvB9cLSnKmvO2mcoA39Suvv6c.QX2cDM1wCOwMzNzEzW}

Bash

'''hacker@path\~the-path-variable:\~$ PATH=" "        
hacker@path\~the-path-variable:\~$ /challenge/run             
Trying to remove /flag...             
/challenge/run: line 4: rm: command not found               
The flag is still there! I might as well give it to you!               
pwn.college{s0QvB9cLSnKmvO2mcoA39Suvv6c.QX2cDM1wCOwMzNzEzW}'''             


## Notes And Errors:
None.

## References:
None.
