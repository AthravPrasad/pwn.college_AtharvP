# Becoming Root with su


## My Solve:
I used the su (substitute user) command without any arguments to attempt to switch to the root user.
Once I gained the root shell, I used cat /flag to read the flag file, which is usually only readable by root.

*Flag:* pwn.college{MTHTQ66ssi9NNkjD5dJesigWU_B.QX1UDN1wCOwMzNzEzW}

Bash

''' hacker@users\~becoming-root-with-su:\~$ su               
Password:         
root@users\~becoming-root-with-su:/home/hacker# cat /flag             
pwn.college{MTHTQ66ssi9NNkjD5dJesigWU_B.QX1UDN1wCOwMzNzEzW}'''             


## Notes and Errors:
None.

## References:
None.
