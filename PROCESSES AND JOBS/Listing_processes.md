# Listing and Identifying a Target Process with ps

## My Solve:
I used the ps command with the -ef and aux options to list all running processes and identify the flag-generating challenge executable. 
The process list clearly showed the program /challenge/29184-run-4546 running as root. By executing this program directly, the flag was revealed before it terminated or went to sleep.

*Flag:* pwn.college{8sA9LWDCVBRBOZNgzUqnpMmaavS.QX4MDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~listing-processes:~$ ps -ef
UID           PID  PPID  C STIME TTY          TIME CMD
...
root          132     1  0 13:43 ?        00:00:00 /challenge/29184-run-4546
...
hacker@processes\~listing-processes:~$ /challenge/29184-run-4546
Yahaha, you found me! Here is your flag:
pwn.college{8sA9LWDCVBRBOZNgzUqnpMmaavS.QX4MDO0wCOwMzNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').'''


## Notes and Errors:
None.

## References:
None.
