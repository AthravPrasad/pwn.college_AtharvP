# Resuming Processes with fg


## My Solve:
I executed the /challenge/run program and used the Ctrl-Z key combination to suspend the process, moving it to the background job list. 
This action sends the SIGTSTP signal. I then used the fg (foreground) command without arguments to bring the most recently suspended job back into the foreground. 
Resuming the process allowed it to complete its execution and print the flag.

*Flag:* pwn.college{0YWjlvmKY4QE49WpJ9b3MC4injv.QX2QDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~resuming-processes:\~$ /challenge/run                         
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with               
the 'fg' command! Or just press Enter to quit me!            
^Z          
[1]+  Stopped                 /challenge/run            
hacker@processes\~resuming-processes:~$ fg           
/challenge/run                
I'm back! Here's your flag:        
pwn.college{0YWjlvmKY4QE49WpJ9b3MC4injv.QX2QDO0wCOwMzNzEzW}'''           
Don't forget to press Enter to quit me!          

Goodbye!            


## Notes and Errors:
None.

## References:
None.
