# Reading Shell Scripts


## My Solve
The challenge requires reading the /challenge/run shell script using the cat command to understand its logic.
The script checks if the user's input (read into the variable GUESS) is exactly equal to the string "hack the PLANET".
By piping the correct password directly to the /challenge/run program, the condition is met, and the script prints the flag.

*Flag:* pwn.college{8kMe1A_ZX2z2lxXqfqUfks3qLKX.0lMwgDOxwCOwMzNzEzW}

Bash

hacker@chaining\~reading-shell-scripts:\~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if \[ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining\~reading-shell-scripts:\~$ echo "hack the PLANET" | /challenge/run
CORRECT! Your flag:
pwn.college{8kMe1A_ZX2z2lxXqfqUfks3qLKX.0lMwgDOxwCOwMzNzEzW}


## Notes And Errors:
None

## References:
None
