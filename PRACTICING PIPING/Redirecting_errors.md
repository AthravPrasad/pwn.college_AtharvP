# Redirecting Errors

## My Solve:
I used the append redirection operator (>>) to direct the program's standard output (stdout) to the file myflag.
Simultaneously, I used the file descriptor 2> to direct the program's standard error (stderr) to the file instructions.
This captured the flag in myflag and the success messages in instructions.

*Flag:* pwn.college{0Nof54mvIIYA6AQNVBDYq453V2-.QX3YTN0wCOwMzNzEzW}

Bash

hacker@piping\~redirecting-errors:~$ /challenge/run >> myflag 2> instructions
hacker@piping\~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oDhz_Nb3K8Ok8F6Fh4QOPHpnJff.QX1YTN0wCOwMzNzEzW}


[FLAG] Here is your flag:
[FLAG] pwn.college{0Nof54mvIIYA6AQNVBDYq453V2-.QX3YTN0wCOwMzNzEzW}

hacker@piping\~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping\~redirecting-errors:~$

## Notes and Errors:
None.

## References:
None.







