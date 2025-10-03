# Using sudo to Read Root Files


## My Solve:
Since the hacker user is configured to run this specific command (or commands in general) as root without needing a password in this environment, this action bypassed the file's permission restrictions and allowed me to read the flag.

*Flag:* pwn.college{Es6RoarnVxdzbn1_AXrEgHkt8b5.QX4UDN1wCOwMzNzEzW}

Bash

'''hacker@users\~using-sudo:~$ sudo cat /flag                       
pwn.college{Es6RoarnVxdzbn1_AXrEgHkt8b5.QX4UDN1wCOwMzNzEzW}'''           


## Notes and Errors:
None.

## References:
None.
