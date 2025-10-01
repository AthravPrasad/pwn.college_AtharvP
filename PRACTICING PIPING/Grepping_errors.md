# Grepping Errors

## My Solve:
The challenge required that the standard error (stderr) output of /challenge/run be piped directly into the grep command.
I used 2>&1 to redirect file descriptor 2 (stderr) to file descriptor 1 (stdout). The resulting combined stream (stdout + stderr) was then piped via | into grep pwn.college, successfully filtering the live stderr output and extracting the flag.

*Flag:* pwn.college{UdtvsbPaVO3zDqZQNasQmpAV9LU.QX1ATO0wCOwMzNzEzW}

Bash

hacker@piping\~grepping-errors:~$ /challenge/run 2>&1 | grep pwn.college      
[INFO] WELCOME! This challenge makes the following asks of you:                             
[INFO] - the challenge checks for a specific process at the other end of stderr : grep            
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt       

[HYPE] ONWARDS TO GREATNESS!                             

[INFO] This challenge will perform a bunch of checks.                               
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.         

[TEST] You should have redirected my stderr to another process. Checking...         
[TEST] Performing checks on that process!          

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.            
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).        
[INFO] To pass the checks, the executable must be grep.           

[PASS] You have passed the checks on the process on the other end of my stderr!       
[PASS] Success! You have satisfied all execution requirements.     
pwn.college{UdtvsbPaVO3zDqZQNasQmpAV9LU.QX1ATO0wCOwMzNzEzW}        
hacker@piping\~grepping-errors:~$           


## Notes and Errors:
None.

## References:
None.
