# Changing File Ownership (Permissions)

## My Solve:
I exploited a capability or misconfiguration that allowed the hacker user to use the chown command on a file owned by root.
By changing the ownership of /flag to hacker, I gained the necessary permissions to use the cat command to read the file's contents.

*Flag:* pwn.college{EclW7EXvVCuHZKnZ41txK7hAI5L.QXxEjN0wCOwMzNzEzW}

Bash

'''hacker@permissions~changing-file-ownership:\~$ ls -l /flag                      
-r-------- 1 root root 60 Oct 11 11:11 /flag                                
hacker@permissions\~changing-file-ownership:\~$ chown hacker /flag                  
hacker@permissions\~changing-file-ownership:\~$ ls -l /flag                  
-r-------- 1 hacker root 60 Oct 11 11:11 /flag                   
hacker@permissions\~changing-file-ownership:\~$ cat /flag                 
pwn.college{EclW7EXvVCuHZKnZ41txK7hAI5L.QXxEjN0wCOwMzNzEzW}'''                         


## Notes and Errors:
None.

## References:
None.
