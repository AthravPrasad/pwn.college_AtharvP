# Redirecting Input

## My Solve:
I first created the file PWN containing the string COLLEGE. I then used the input redirection operator (<) to pass the content of PWN as standard input to the /challenge/run program, getting the flag.

*Flag:* pwn.college{I8B3de0E6IFkurCm-BLG1Nv-4Db.QXwcTN0wCOwMzNzEzW}

Bash

hacker@piping\~redirecting-input:~$ echo COLLEGE >> PWN         
hacker@piping\~redirecting-input:~$ /challenge/run < PWN            
Reading from standard input...          
Correct! You have redirected the PWN file into my standard input, and I read       
the value 'COLLEGE' out of it!              
Here is your flag:             
pwn.college{I8B3de0E6IFkurCm-BLG1Nv-4Db.QXwcTN0wCOwMzNzEzW}          
hacker@piping\~redirecting-input:~$      

## Notes and Errors:
None.

## References:
None.
