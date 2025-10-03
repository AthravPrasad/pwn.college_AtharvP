# Extracting the First Lines with head


## My Solve:
I used the head command to extract a specific number of lines from the output of the first executable, /challenge/pwn, and piped the result into the second executable, /challenge/college.
This did the job.

*Flag:* pwn.college{Mh2uGUQlBvxodX776kyrTSTcCRB.0lNxEzNxwCOwMzNzEzW}

Bash

'''hacker@data\~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{Mh2uGUQlBvxodX776kyrTSTcCRB.0lNxEzNxwCOwMzNzEzW}'''


## Notes and Errors:
None.

## References:
None.
