# Listing Files 

## My Solve:
Firstly located which file was impersonating run by using ls in chaLLenge directory.      
Then Invoked it.

*Flag:* pwn.college{86RVfnRR59t1CdRxyn-aibQhdg1.QX4IDO0wCOwMzNzEzW}

bash \
hacker@commands\~listing-files:\~$ ls /challenge           
14545-renamed-run-20572  DESCRIPTION.md              
hacker@commands\~listing-files:\~$ cat 14545-renamed-run-20572             
cat: 14545-renamed-run-20572: No such file or directory               
hacker@commands~listing-files:\~$ /challenge/14545-renamed-run-20572                      
Yahaha, you found me! Here is your flag:            
pwn.college{86RVfnRR59t1CdRxyn-aibQhdg1.QX4IDO0wCOwMzNzEzW}                     
                      
## Notes And Errors :
Tried to read an executable file like text.

## References:
None.

