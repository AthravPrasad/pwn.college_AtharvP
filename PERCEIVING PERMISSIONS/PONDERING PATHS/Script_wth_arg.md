# Scripting with Arguments


## My Solve:
The objective was to create a script that accepts two command-line arguments and prints them in reverse order. This requires using the positional parameters $1 and $2 in a non-sequential manner within the script body.
I created the script /home/hacker/solve.sh using the cat command with a here document.
The script's core logic used printf to print the second argument ($2) followed by the first argument ($1). The double quotes ensured that the arguments were treated as distinct strings, separated by a space.
I made the script executable with chmod +x.
After correcting a typo in the challenge binary path (/CHALLENGE/RUN to /challenge/run), running the checker successfully verified the argument reversal and retrieved the flag.

*Flag:* pwn.college{cepciE8R3dQkGpVE_nuZXkEmnn9.0VNzMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~scripting-with-arguments:\~$ cat > /home/hacker/solve.sh <<'EOF' 
> #!/bin/bash                  
> printf '%s %s\n' "$2" "$1"     
> EOF
hacker@chaining\~scripting-with-arguments:\~$ chmod +x /home/hacker/solve.sh        
hacker@chaining\~scripting-with-arguments:\~$ /CHALLENGE/RUN        
bash: /CHALLENGE/RUN: No such file or directory                  
hacker@chaining\~scripting-with-arguments:\~$ /challenge/run        
Correct! Your script properly reversed the arguments.         
Here's your flag:          
pwn.college{cepciE8R3dQkGpVE_nuZXkEmnn9.0VNzMDOxwCOwMzNzEzW}            


## Notes And Errors:
None(really).


## References:
None.
