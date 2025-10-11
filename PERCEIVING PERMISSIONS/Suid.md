# The SUID Bit


## My Solve:
The objective was to gain elevated privileges (root) by manipulating the special SUID permission bit on the executable /challenge/getroot.
I used the chmod command in symbolic mode (u+s) to set the SUID bit for the user owner (u).
Setting the SUID bit causes the program to run with the permissions of the file's owner, regardless of who executes it. Since the file was owned by root, executing it ran the provided shell command with root privileges.
Once the root shell was obtained, I used cat on the protected /flag file to retrieve the final flag.

*Flag:* pwn.college{kTId-waTEW50hnp_sxzrwvyVrd7.QXzEjN0wCOwMzNzEzW}

Bash

'''hacker@permissions\~the-suid-bit:\~$ chmod u+s /challenge/getroot
hacker@permissions\~the-suid-bit:\~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root! 
Here is your shell...
root@permissions\~the-suid-bit:\~# cat /flag
pwn.college{kTId-waTEW50hnp_sxzrwvyVrd7.QXzEjN0wCOwMzNzEzW}'''


## Notes And Errors:
The SUID bit is a critical security concept. When set on a binary, it allows a low-privilege user (like hacker) to temporarily run that program with the privileges of the file owner (in this case, root).

## References:
None.








