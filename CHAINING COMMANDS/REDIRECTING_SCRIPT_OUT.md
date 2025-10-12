# Redirecting Script Output


## My Solve:
The objective was to run a shell script that executes two programs and then pipe the combined output of those programs directly into a third program, /challenge/solve.
I used the cat command with a here document (<<'EOF') to create the script file x.sh containing the two executable calls: /challenge/pwn and /challenge/college.
I then used the pipe operator (|) to take the standard output of the script (bash x.sh) and redirect it as the standard input for the /challenge/solve program, successfully completing the challenge.

*Flag:* pwn.college{kMbRSp_7YKUlxjBIOwGfcDJ7WGO.QX4ETO0wCOwMzNzEzW}

Bash

'''hacker@chaining\~redirecting-script-output:\~$ cat > x.sh <<'EOF'          
> /challenge/pwn 
> /challenge/college
> EOF                
hacker@chaining\~redirecting-script-output:\~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{kMbRSp_7YKUlxjBIOwGfcDJ7WGO.QX4ETO0wCOwMzNzEzW}

## Notes And Errors:
None.

## References:
None.
