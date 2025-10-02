# Splitting Pipes for STDERR and STDOUT

## My Solve:
Used **`bash` file descriptor redirection** and **process substitution (`>()`)** to send **STDOUT** to `/challenge/planet` and **STDERR** to `/challenge/the` simultaneously.

*Flag:* pwn.college{ksjdYg4MOTSP0Qz5nbtK8Nge_B7.QXxQDM2wCOwMzNzEzW}

bash
''' hacker@piping\~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )          
Congratulations, you have learned a redirection technique that even experts           
struggle with! Here is your flag:        
pwn.college{ksjdYg4MOTSP0Qz5nbtK8Nge_B7.QXxQDM2wCOwMzNzEzW} '''          

## Notes and Errors:
None.

## References:
None.
