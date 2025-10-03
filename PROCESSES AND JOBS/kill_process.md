# Killing a Blocking Process

## My Solve:
I used the ps aux command to list all running processes and identified the program named /challenge/dont_run, which was likely blocking the execution of /challenge/run. 
This blocking process was running under PID 136. I then used the kill command on this PID to terminate the process, which allowed the /challenge/run executable to execute successfully and output the flag.

*Flag:* pwn.college{YifuFZYIpcV0JcO04Nr45P5SCG0.QXyQDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~killing-processes:~$ ps aux                                   
USER          PID %CPU %MEM    VSZ   RSS TTY      STAT START      TIME COMMAND                     
...             
hacker        136  0.0  0.0 231576  3520 ?        Ss   14:00      0:00 /challenge/dont_run               
...               
hacker@processes\~killing-processes:~$ kill 136            
hacker@processes\~killing-processes:~$ /challenge/run             
Great job! Here is your payment:                                 
pwn.college{YifuFZYIpcV0JcO04Nr45P5SCG0.QXyQDO0wCOwMzNzEzW}...                      


## Notes and Errors:
None.

## References:
None.
