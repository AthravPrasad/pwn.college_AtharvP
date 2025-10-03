# Foregrounding a Backgrounded Process


## My Solve:
I followed the instructions by first executing /challenge/run and suspending it with Ctrl-Z.
Next, I used the bg (background) command to resume the suspended job, allowing it to run actively in the background.
Finally, I used the fg (foreground) command to bring the backgrounded job back to the foreground. This sequence satisfied the challenge requirement and revealed the flag.

*Flag:* pwn.college{YK86KX2mOVVRom85B4RjTu3iC8L.QX4QDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~foregrounding-processes:~$ /challenge/run                      
To pass this level, you need to suspend me, resume the suspended process in the              
background, and *then* foreground it without re-suspending it! You can               
background me with Ctrl-Z (and resume me in the background with 'bg') or, if              
you're not ready to do that for whatever reason, just hit Enter and I'll exit!           
^Z                  
[1]+  Stopped                  /challenge/run                      
hacker@processes\~foregrounding-processes:~$ bg /challenge/run          
[1]+ /challenge/run &            
hacker@processes\~foregrounding-processes:~$ fg /challenge/run           
/challenge/run 
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!                  

pwn.college{YK86KX2mOVVRom85B4RjTu3iC8L.QX4QDO0wCOwMzNzEzW}               


## Notes and Errors:
None.

## References:
None.
