# Finding Commands


## My Solve:
The objective was to locate the directory containing a hidden command, which would be on the system's execution path. I used the which utility, followed by the command name (win), to output the full path of the executable.
The which win command revealed the path: /challenge/paths/9982/win.
Knowing the directory, I used ls to inspect the contents of /challenge/paths/9982, which showed both the win executable and the hidden flag file.
Finally, I used cat on the absolute path to the flag file to retrieve the flag.

*Flag:* pwn.college{4pQudsWl2wLpkp_aSQKj8oROW9l.01NzEzNxwCOwMzNzEzW}

Bash

'''hacker@path\~finding-commands:\~$ which win
/challenge/paths/9982/win
hacker@path\~finding-commands:\~$ ls /challenge/paths/9982
flag win
hacker@path\~finding-commands:\~$ cat /challenge/paths/9982/flag
pwn.college{4pQudsWl2wLpkp_aSQKj8oROW9l.01NzEzNxwCOwMzNzEzW}'''


## Notes And Errors:
None.

## References:
None.







