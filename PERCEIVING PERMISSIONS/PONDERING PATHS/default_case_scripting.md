# Scripting with Default Cases (if/else)


## My Solve:
The objective was to create a script that implemented a complete conditional check using an if/else block: outputting "college" for a specific input ("pwn") and a different default output ("nope") for any other input.
I created the script /home/hacker/solve.sh using cat with a here document.
The script included a full if/else block: it checks if the first argument ($1) equals "pwn"; if true, it executes the if block, otherwise it executes the else block, ensuring all inputs are handled.
I used chmod +x to make the script executable.
Running /challenge/run successfully verified that both the positive condition and the default case were handled correctly, and retrieved the flag.

*Flag:* pwn.college{4p9tgtkqxu9iQ4BgVZnU7iGp7pd.01NzMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~scripting-with-default-cases:~$ cat > /home/hacker/solve.sh <<'EOF'           
> #!/bin/bash                    
> if \[ "$1" = "pwn" ]; then         
>    printf '%s\n' 'college'                
> else                   
>    printf '%s\n' 'nope'             
> fi        
> EOF      
hacker@chaining\~scripting-with-default-cases:\~$ chmod +x /home/hacker/solve.sh        
hacker@chaining\~scripting-with-default-cases:\~$ /challenge/run             
Correct! Your script properly handles the if/else conditions.          
Here's your flag:       
pwn.college{4p9tgtkqxu9iQ4BgVZnU7iGp7pd.01NzMDOxwCOwMzNzEzW}''' 


## Notes And Errors:
None.

## References:
None.







