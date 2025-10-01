# Matching Paths With Bracket Globbing

## My Solve:
Firstly, I used a bracket glob ([bash]) to match any one of the characters b, a, s, or h.
After correcting the invocation to use the correct path /challenge/files/file_[bash], the challenge accepted the expansion and printed the flag.

*Flag:* pwn.college{sZP_5SgEeGRhDv8vTEo4togUi_m.QX0IDO0wCOwMzNzEzW}

bash \
''' hacker@globbing~matching-paths-with-:~$ /challenge/run/file_[bash]
bash: /challenge/run/file_[bash]: Not a directory
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/files_[bash]
Your expansion did not expand to the requested files (/challenge/files/file_b, 
/challenge/files/file_a, /challenge/files/file_s, and /challenge/files/file_h). 
Instead, it expanded to:
/challenge/files/files_[bash]
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{sZP_5SgEeGRhDv8vTEo4togUi_m.QX0IDO0wCOwMzNzEzW}'''

## Notes and Errors:

Simple typo.

## References:

None.
