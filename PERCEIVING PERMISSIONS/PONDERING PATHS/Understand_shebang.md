# Understanding Shebangs


## My Solve:
This challenge required creating an executable script with a proper shebang that produces specific output, demonstrating an understanding of how shebangs determine the script's interpreter.
I used the cat command with a here document (<<'EOF') to create the file /home/hacker/solve.sh.
The script was given a specific shebang line (#!/bin/bash) to ensure it was executed by the Bash interpreter.
The script used the printf command to output the required string: hack the planet.
I then used chmod +x to grant executable permission.
Running /challenge/run successfully executed our script using the specified interpreter, granting the flag.

*Flag:* pwn.college{QeH24lBrHYdWzzE12zDwDWc3u1K.0VOzMDOxwCOwMzNzEzW}

Bash

'''hacker@chaining\~understanding-shebangs:\~$ cat > /home/hacker/solve.sh <<'EOF'             
> #!/bin/bash                       
> printf '%s\n' 'hack the planet'            
> EOF                 
hacker@chaining\~understanding-shebangs:\~$ chmod +x /home/hacker/solve.sh          
hacker@chaining\~understanding-shebangs:\~$ /challenge/run          
Testing your script...              
Perfect! Your flag:           
Flag: pwn.college{QeH24lBrHYdWzzE12zDwDWc3u1K.0VOzMDOxwCOwMzNzEzW}'''          


## Notes And Errors:
None.

## References:
None.







