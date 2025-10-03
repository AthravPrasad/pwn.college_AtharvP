# Backgrounding and Detecting a Running Process


## My Solve:
I began by executing the first instance and suspending it with Ctrl-Z. I then used the bg (background) command to resume the suspended job in the background, allowing it to continue running.
Finally, I executed the second instance of /challenge/run, which successfully detected the backgrounded process and printed the flag.

*Flag:* pwn.college{wkBAZwLQbHVO7NIuVjFTeEty_5t.QX3QDO0wCOwMzNzEzW}

Bash

hacker@processes\~backgrounding-processes:\~$ /challenge/run                       
I'll only give you the flag if there's already another copy of me running *and                
not suspended* in this terminal... Let's check!              
 
UID           PID STAT CMD                    
root          165 S+   bash /challenge/run              
root          167 R+   ps -o user=UID,pid,stat,cmd            

I don't see a second me!            

To pass this level, you need to suspend me, resume the suspended process in the                 
background, and then launch a new version of me! You can background me with               
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to               
do that for whatever reason, just hit Enter and I'll exit!               
^Z
[1]+  Stopped                 /challenge/run                 
hacker@processes\~backgrounding-processes:\~$ bg               
[1]+ /challenge/run &                         
hacker@processes\~backgrounding-processes:\~$ /challenge/run                        
I'll only give you the flag if there's already another copy of me running *and                 
not suspended* in this terminal... Let's check!              
 
UID           PID STAT CMD                      
root          165 S    bash /challenge/run            
root          175 S    sleep 6h               
root          176 S+   bash /challenge/run            
root          178 R+   ps -o user=UID,pid,stat,cmd           

Yay, I found another version of me running in the background! Here is the flag:            
pwn.college{wkBAZwLQbHVO7NIuVjFTeEty_5t.QX3QDO0wCOwMzNzEzW}             


## Notes and Errors: 
None.

## References:
None.
