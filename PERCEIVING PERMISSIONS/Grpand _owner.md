# Groups and Files (Group Ownership)

## My Solve:
The file /flag was previously unreadable, but I was able to successfully execute the chgrp hacker /flag command.
This changed the file's group owner to my primary group, hacker.
Since the file likely had read permissions for its group, this change granted me the necessary access to read the flag using cat /flag.

*Flag:* pwn.college{IQH4loCMc0E9ADDH_zIJ6Fi3Gn4.QXxcjM1wCOwMzNzEzW}

Bash

'''hacker@permissions\~groups-and-files:\~$ chgrp hacker /flag             
hacker@permissions\~groups-and-files:\~$ cat /flag              
pwn.college{IQH4loCMc0E9ADDH_zIJ6Fi3Gn4.QXxcjM1wCOwMzNzEzW}            

## Notes and Errors:
None.

## References:
None.

