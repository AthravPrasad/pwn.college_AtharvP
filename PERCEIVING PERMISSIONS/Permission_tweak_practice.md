# Permission Tweaking Practice

## My Solve:
The challenge presented 8 rounds, each requiring me to use the chmod command to change the permissions of the file /challenge/pwn to match a specified target set.
I utilized the symbolic mode in chmod to precisely add, remove, or set permissions for the user (u), group (g), and others (o).
After successfully completing all 8 rounds, the final step was to set read permissions on the /flag file, which was initially inaccessible, and then use cat to retrieve the flag.
For this final step, I used octal mode (400) to grant read permission only to the user.

*Flag*: pwn.college{EFbpPYNtgdMsvb3M7cDB5hyFciy.QXwEjN0wCOwMzNzEzW}

Bash

hacker@permissions\~permission-tweaking-practice:\~$ /challenge/run
Round 1 of 8!

Current permissions of "/challenge/pwn": rw-r--r--
...
Needed permissions of "/challenge/pwn": rwxr--r-x
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=rwx,g=r,o=rx /challenge/pwn
You set the correct permissions!
Round 2 of 8!

Current permissions of "/challenge/pwn": rwxr--r-x
...
Needed permissions of "/challenge/pwn": rwxr-xr-x
hacker@permissions\~permission-tweaking-practice:\~$ chmod g+x /challenge/pwn
You set the correct permissions!
Round 3 of 8!

Current permissions of "/challenge/pwn": rwxr-xr-x
...
Needed permissions of "/challenge/pwn": --xr-x--x
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=x,g=rx,o=x /challenge/pwn
You set the correct permissions!
Round 4 of 8!

Current permissions of "/challenge/pwn": --xr-x--x
...
Needed permissions of "/challenge/pwn": rwxr-xrwx
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=rwx,g=rx,o=rwx /challenge/pwn
You set the correct permissions!
Round 5 of 8!

Current permissions of "/challenge/pwn": rwxr-xrwx
...
Needed permissions of "/challenge/pwn": rwx--x-wx
hacker@permissions\~permission-tweaking-practice:\~$ chmod g-r,o-r /challenge/pwn
You set the correct permissions!
Round 6 of 8!

Current permissions of "/challenge/pwn": rwx--x-wx
...
Needed permissions of "/challenge/pwn": r------wx
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=r,g=,o=wx /challenge/pwn
You set the correct permissions!
Round 7 of 8!

Current permissions of "/challenge/pwn": r------wx
...
Needed permissions of "/challenge/pwn": r-----rwx
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=r,g=,o=rwx /challenge/pwn
You set the correct permissions!
Round 8 of 8!

Current permissions of "/challenge/pwn": r-----rwx
...
Needed permissions of "/challenge/pwn": -------w-
hacker@permissions\~permission-tweaking-practice:\~$ chmod u=,g=,o=w /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------
...
hacker@permissions\~permission-tweaking-practice:\~$ chmod 400 /flag
hacker@permissions\~permission-tweaking-practice:\~$ cat /flag
pwn.college{EFbpPYNtgdMsvb3M7cDB5hyFciy.QXwEjN0wCOwMzNzEzW}

## Notes And Errors:
None.

## References:
None.
