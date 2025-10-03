# Starting Processes Directly in the Background

## My Solve:
I executed the /challenge/run program and started it directly in the background by appending the ampersand symbol (&) to the command.

*Flag:* pwn.college{wldn3Hqzt1opVeyPr05cCi7lJNI.QX5QDO0wCOwMzNzEzW}

Bash

'''hacker@processes\~starting-backgrounded-processes:\~$ /challenge/run              
You've started me in the foreground! You must start me in the background (by               
appending '&' to the command) to get the flag!          
hacker@processes\~starting-backgrounded-processes:\~$ /challenge/run &           
[1] 151         
hacker@processes\~starting-backgrounded-processes:\~$           

Yay, you started me in the background! Because of that, this text will probably           
overlap weirdly with the shell prompt, but you're used to that by now...             
         
Anyways! Here is your flag!       
pwn.college{wldn3Hqzt1opVeyPr05cCi7lJNI.QX5QDO0wCOwMzNzEzW}           


## Notes and Errors:
None.

## References:
None.
