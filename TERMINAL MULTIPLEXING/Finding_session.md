# Multiple Screen Sessions


## My Solve:
The objective was to check multiple detached screen sessions to locate the single session containing the flag. This requires listing available sessions, attaching to them, reading the output, and detaching to continue checking.
I used screen -ls (or screen -list) to show all available detached sessions and their IDs. I then attempted to attach to each one.
I attached to the first session using screen -r <ID>, found it was a decoy, and detached using Ctrl+A d.
I attached to the second session, which contained the output of the challenge program and displayed the flag.

*Flag:* pwn.college{th3sdffl4gnb15wq1nzc4n0th3r56jfw1nd0w4lw4y5.0V8cDM0wCOwMzNzEzW}

Bash

'''hacker@terminal-multiplexing\~multiple-sessions:~$ screen -ls
There are screens on:
123.pts-0.terminal-multiplexing~multiple-sessions (Detached)
456.pts-0.terminal-multiplexing~multiple-sessions (Detached)
789.pts-0.terminal-multiplexing~multiple-sessions (Detached)
3 Sockets in /run/screen/S-hacker.

hacker@terminal-multiplexing\~multiple-sessions:\~$ screen -r 456
Detaching from screen:
\[Previous Output from challenge here]
Welcome to the decoy! Try another session.
\[Ctrl-A d pressed]

hacker@terminal-multiplexing\~multiple-sessions:\~$ screen -r 789
Detaching from screen:
\[Previous Output from challenge here]
Congratulations! You found the right session!
pwn.college{th3sdffl4gnb15wq1nzc4n0th3r56jfw1nd0w4lw4y5.0V8cDM0wCOwMzNzEzW}'''

## Notes And Errors:
The challenge relies on the screen -ls command to list session identifiers (123, 456, 789) and screen -r <ID> to attach to a specific one. The manual detachment using Ctrl+A d is critical to keep the other sessions running in the background.

## References:
None.







