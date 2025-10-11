# Scripting with Multiple Conditions (case Statement)


## My Solve:
The objective was to create an executable shell script that handles several specific string inputs, each requiring a unique output, while also defining a default output for all other inputs. This was accomplished efficiently using the case statement.
I created the script /home/hacker/solve.sh using the cat command with a here document.
The script implements a case block that checks the value of the first argument ($1) against patterns like hack), pwn), and learn).
The special *) pattern was used to define the default case, outputting "unknown" for any unmatched input.
I used chmod +x to grant executable permission.
Running /challenge/run verified that the script correctly matched all specified conditions and handled the default case, granting the flag.


*Flag:* pwn.college{kGNZfuzxdf_LcQlph56Va3PW5nF.0FOzMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~scripting-with-multiple-conditions:\~$ cat > /home/hacker/solve.sh <<'EOF'
> #!/bin/bash
> case "$1" in
> hack) printf '%s\n' 'the planet' ;;
> pwn) printf '%s\n' 'college' ;;
> learn) printf '%s\n' 'linux' ;;
> *) printf '%s\n' 'unknown' ;;
> esac
> EOF
hacker@chaining\~scripting-with-multiple-conditions:\~$ chmod +x /home/hacker/solve.sh
hacker@chaining\~scripting-with-multiple-conditions:\~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{kGNZfuzxdf_LcQlph56Va3PW5nF.0FOzMDOxwCOwMzNzEzW}'''


## Notes And Errors:
None.

## References:
None.
