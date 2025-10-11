# Permissions Setting Practice


## My Solve:
This challenge involved 8 rounds of permission manipulation, requiring precise adjustments to the access rights of the file /challenge/pwn using chmod. 
I primarily used the symbolic mode in chmod (e.g., u=rwx, g+x, o-w) to explicitly set, add, or remove permissions for the owner (u), group (g), and others (o).
After successfully matching the permissions for all 8 rounds, the final step required granting read access to the /flag file, whose ownership was transferred to me. I used octal mode (400) to give the current user read-only access and then used cat to view the flag.

*Flag:* pwn.college{QtN6t4dnXfOKHf0Dq9FKWAIeEDe.QXzETO0wCOwMzNzEzW}

Bash

'''hacker@permissions\~permissions-setting-practice:\~$ chmod u=r,g=w,o=r /challenge/pwn
You set the correct permissions!
Round 2 of 8!

Current permissions of "/challenge/pwn": r---w-r--
...
Needed permissions of "/challenge/pwn": r--r-x-w-
hacker@permissions\~permissions-setting-practice:\~$ chmod u=r,g=rx,o=w /challenge/pwn
You set the correct permissions!
Round 3 of 8!

Current permissions of "/challenge/pwn": r--r-x-w-
...
Needed permissions of "/challenge/pwn": -w-----w-
hacker@permissions\~permissions-setting-practice:\~$ chmod u=w,g=,o=w /challenge/pwn
You set the correct permissions!
Round 4 of 8!

Current permissions of "/challenge/pwn": -w-----w-
...
Needed permissions of "/challenge/pwn": r-xr-xr-x
hacker@permissions\~permissions-setting-practice:\~$ chmod u=rx,g=rx,o=rx /challenge/pwn
You set the correct permissions!
Round 5 of 8!

Current permissions of "/challenge/pwn": r-xr-xr-x
...
Needed permissions of "/challenge/pwn": -wx--x-wx
hacker@permissions\~permissions-setting-practice:\~$ chmod u=wx,g=x,o=wx /challenge/pwn
You set the correct permissions!
Round 6 of 8!

Current permissions of "/challenge/pwn": -wx--x-wx
...
Needed permissions of "/challenge/pwn": r---w-rwx
hacker@permissions\~permissions-setting-practice:\~$ chmod u=r,g=w,o=rwx /challenge/pwn
You set the correct permissions!
Round 7 of 8!

Current permissions of "/challenge/pwn": r---w-rwx
...
Needed permissions of "/challenge/pwn": rwx-wxrwx
hacker@permissions\~permissions-setting-practice:\~$ chmod u=rwx,g=wx,o=rwx /challenge/pwn
You set the correct permissions!
Round 8 of 8!

Current permissions of "/challenge/pwn": rwx-wxrwx
...
Needed permissions of "/challenge/pwn": rw---x-w-
hacker@permissions\~permissions-setting-practice:\~$ chmod u=rw,g=x,o=w /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------
...
hacker@permissions\~permissions-setting-practice:\~$ chmod 400 /flag
hacker@permissions\~permissions-setting-practice:\~$ cat /flag
pwn.college{QtN6t4dnXfOKHf0Dq9FKWAIeEDe.QXzETO0wCOwMzNzEzW}


## Notes And Errors:
None.


## References:
None.
