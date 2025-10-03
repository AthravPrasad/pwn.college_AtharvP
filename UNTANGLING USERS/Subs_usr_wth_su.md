# Substituting User with su


## My Solve:
I used the su (substitute user) command and specified the username zardus as an argument. 
After successfully changing users, I executed the /challenge/run program, which printed the flag reserved for the zardus user.

*Flag:* pwn.college{wSsjM5lvKY3aamex6taE9fwy_7L.QX2UDN1wCOwMzNzEzW}

Bash

'''hacker@users\~other-users-with-su:~$ su zardus      
Password:          
zardus@users\~other-users-with-su:/home/hacker$ /challenge/run         
Congratulations, you have become Zardus! Here is your flag:          
pwn.college{wSsjM5lvKY3aamex6taE9fwy_7L.QX2UDN1wCOwMzNzEzW}'''       


## Notes and Errors:
None.

## References:
None.
