# Linking Files

## My Solve:
The challenge required creating a symbolic link named /home/hacker/not-the-flag that pointed to the flag file at /flag. 
I first deleted the existing file using rm, then used the ln -s command to create the symbolic link. 
Running /challenge/catflag then followed the link and printed the flag.

*Flag:* pwn.college{AwV3Jy_EQ5m4HhdJjQ9txig2dbV.QX5ETN1wCOwMzNzEzW}

Bash

hacker@commands\~linking-files:\~$ ln -s /flag /home/hacker/not-the-flag         
ln: failed to create symbolic link '/home/hacker/not-the-flag': File exists        
hacker@commands\~linking-files:\~$ rm /home/hacker/not-the-flag            
hacker@commands\~linking-files:\~$ ln -s /flag /home/hacker/not-the-flag           
hacker@commands\~linking-files:\~$ /challenge/catflag            
About to read out the /home/hacker/not-the-flag file!
pwn.college{AwV3Jy_EQ5m4HhdJjQ9txig2dbV.QX5ETN1wCOwMzNzEzW}


## Notes and Errors:
I first encountered an error because the target file already existed. 
I used the rm command to remove the existing file before successfully creating the symbolic link.

## References:
None.
