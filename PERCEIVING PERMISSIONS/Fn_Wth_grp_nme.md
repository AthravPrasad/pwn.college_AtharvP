# Fun With Group Names (Targeted Group Change)

## My Solve:
I first checked my current primary Group ID (GID) using the id command and confirmed the group name with id -gn, which was grp30835.
The file permissions indicated read access for the group owner (-r--r-----).
Therefore, I used the chgrp command to change the group ownership of /flag to grp30835. 
This granted me the required group read permission, allowing me to retrieve the flag with cat /flag.

*Flag:* pwn.college{sJoVkBUkrDF27NQvEbGY2OvqCLK.QXycjM1wCOwMzNzEzW}

Bash

'''hacker@permissions\~fun-with-groups-names:\~$ id                     
uid=1000(hacker) gid=1000(grp30835) groups=1000(grp30835)             
hacker@permissions\~fun-with-groups-names:\~$ id -gn              
grp30835           
hacker@permissions\~fun-with-groups-names:\~$ ls -l /flag           
-r--r----- 1 root root 60 Oct 11 11:43 /flag         
hacker@permissions\~fun-with-groups-names:\~$ chgrp grp30835 /flag           
hacker@permissions\~fun-with-groups-names:\~$ cat /flag           
pwn.college{sJoVkBUkrDF27NQvEbGY2OvqCLK.QXycjM1wCOwMzNzEzW}'''           

## Notes and Errors:
None.

## References:
None.

