# Reading Files

## My Solve:
I read the content of the file /challenge/read_me directly into the environment variable PWN using the read command combined with the input redirection operator (<). 
This action set the variable to the file's contents, providing the flag.

*Flag:* pwn.college{ABtiJMcvFJbI9rhoRT6_ZL_EzKF.QXwIDO0wCOwMzNzEzW}

Bash

hacker@variables\~reading-files:~$ read PWN < /challenge/read_me           
You've set the PWN variable properly! As promised, here is the flag:        
pwn.college{ABtiJMcvFJbI9rhoRT6_ZL_EzKF.QXwIDO0wCOwMzNzEzW}          


## Notes and Errors:
None.

## References:
None.
