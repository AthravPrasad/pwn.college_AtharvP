# Tab-completion


## My Solve
The challenge requires using the shell's tab-completion feature to navigate the /challenge/files directory, specifically to find a unique file containing the flag.
By repeatedly typing the next unique character and hitting Tab, the shell auto-completes the path until the flag file is revealed and read with cat.

*Flag:* pwn.college{r34d1ng_th3_c0nt3nt5_0f_th3_f1l35.0VO4IDOxwCOwMzNzEzW}

Bash

'''hacker@commands~tab-complete-for-the-flag:~$ cd /challenge/files        
hacker@commands~files:~$ ls       
pwncollege_A_FILE pwncollege_B_FILE pwncollege_C_FILE pwncollege_FLAG          
hacker@commands~files:~$ cat pwncollege_FLAG                             
pwn.college{r34d1ng_th3_c0nt3nt5_0f_th3_f1l35.0VO4IDOxwCOwMzNzEzW}'''                         


## Notes And Errors:
None

## References:
None
