# Command Chaining with &&

## My Solve:
The objective was to run two commands in sequence: /challenge/first-success and /challenge/second, with the crucial condition that the second command only executes if the first is successful.
I achieved this using the conditional AND operator (&&).

*Flag:* pwn.college{gNquPMd_c2qy8cCR_bHb1bH2DO3.01MOMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~building-on-success:~$ /challenge/first-success && /challenge/second
Nice chaining! Flag: pwn.college{gNquPMd_c2qy8cCR_bHb1bH2DO3.01MOMDOxwCOwMzNzEzW}'''

## Notes And Errors:
None.

## References:
None.
