# Interrupting Processes with Ctrl-C

## My Solve:
I executed the /challenge/run program, which immediately paused and requested an interruption signal to proceed. I pressed Ctrl-C on the keyboard.
This signal interrupted the process, forcing it to exit its waiting loop and print the required flag before terminating.

*Flag:* pwn.college{UXm4BgdtJf-GAInN2CURQCowoV_.QXzQDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~interrupting-processes:\~$ /challenge/run                     
I could give you the flag... but I won't, until this process exits. Remember,               
you can force me to exit with Ctrl-C. Try it now!                            
^C          
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:         
pwn.college{UXm4BgdtJf-GAInN2CURQCowoV_.QXzQDO0wCOwMzNzEzW}'''              


## Notes and Errors:
None.

## References:
None.
