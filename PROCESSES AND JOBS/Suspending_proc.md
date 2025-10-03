# Suspending a Process to Create a Duplicate

## My Solve:
The challenge required two instances of the /challenge/run program to be running simultaneously in the same terminal.
I started the first instance and then used the Ctrl-Z key combination to send a SIGTSTP signal, which suspended the process and moved it to the background.
Then, I launched a second instance of /challenge/run. The second instance detected the suspended first instance and printed the flag.

*Flag:* pwn.college{0AKMbcYCq9HLelpcJUquG0VN-xQ.QX1QDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~suspending-processes:\~$ /challenge/run                  
I'll only give you the flag if there's already another copy of me running in                    
this terminal... Let's check!             

UID           PID  PPID  C STIME TTY          TIME CMD                     
root          147    137  0 15:02 pts/0    00:00:00 bash /challenge/run                   
root          149    147  0 15:02 pts/0    00:00:00 ps -f                                 
 
I don't see a second me!           

To pass this level, you need to suspend me and launch me again! You can            
background me with Ctrl-Z or, if you're not ready to do that for whatever               
reason, just hit Enter and I'll exit!                
^Z
[1]+  Stopped                 /challenge/run               
hacker@processes\~suspending-processes:~$ /challenge/run           
I'll only give you the flag if there's already another copy of me running in                 
this terminal... Let's check!                     

UID           PID  PPID  C STIME TTY          TIME CMD                        
root          147    137  0 15:02 pts/0    00:00:00 bash /challenge/run           
root          154    137  0 15:02 pts/0    00:00:00 bash /challenge/run             
root          156    154  0 15:02 pts/0    00:00:00 ps -f                
 
Yay, I found another version of me! Here is the flag:                      
pwn.college{0AKMbcYCq9HLelpcJUquG0VN-xQ.QX1QDO0wCOwMzNzEzW}                  


## Notes and Errors:                  
None.

## References:
None.
