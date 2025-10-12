# Scripting with Conditional Logic (if)


## My Solve:
The objective was to create an executable script at /home/hacker/solve.sh that implements conditional logic. Specifically, it needed to check if the first argument ($1) was exactly "pwn" and output "college" only in that case.
I created the script file using cat with a here document.
The script uses an if statement to perform a string comparison ([ "$1" = "pwn" ]).
If the condition is true, it executes the echo "college" command.
I used chmod +x to make the script executable.
Running the challenge program verified the script's logic across different test cases and granted the flag.


*Flag:* pwn.college{3X3cut3_th3_1f_st4t3m3nt_c0rr3ctly.0V5cMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~scripting-with-arguments:~$ cat > /home/hacker/solve.sh <<'EOF'
> #!/bin/bash
> if \[ "$1" = "pwn" ]; then
>     echo "college"
> fi
> EOF
hacker@chaining\~scripting-with-arguments:~$ chmod +x /home/hacker/solve.sh
hacker@chaining\~scripting-with-arguments:~$ /challenge/run
Testing your script...
Correct! Your script outputs "college" for "pwn".
Correct! Your script outputs nothing for "foo".
Here's your flag:
pwn.college{3X3cut3_th3_1f_st4t3m3nt_c0rr3ctly.0V5cMDOxwCOwMzNzEzW}'''


## Notes And Errors:
None.

## References:
None.

