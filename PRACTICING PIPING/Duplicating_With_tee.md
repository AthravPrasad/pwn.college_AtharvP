# Duplicating Piped Data with tee

## My Solve:
I used the tee command to duplicate the output stream from /challenge/pwn and save it to interceptor.txt. 
The initial run without arguments printed the usage message containing the required secret code. 
I then used the discovered code (8FYSw70A) to successfully run the commands in the pipeline.

*Flag:* pwn.college{8FYSw70AnqcIfd8s3evYIG9MIKm.QXxITO0wCOwMzNzEzW}

Bash

''' hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee interceptor.txt | /challenge/college
Processing...
WARNING: you are overwriting file interceptor.txt with tee's output...           
The input to 'college' does not contain the correct secret code! This code          
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the            
output of 'pwn' and figure out what the code needs to be.                 
hacker@piping~duplicating-piped-data-with-tee:~$ cat interceptor.txt           
Usage: /challenge/pwn --secret [SECRET_ARG]            

SECRET_ARG should be "8FYSw70A"          
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 8FYSw70A | /challenge/college            
Processing...           
Correct! Passing secret value to /challenge/college...           
Great job! Here is your flag:          
pwn.college{8FYSw70AnqcIfd8s3evYIG9MIKm.QXxITO0wCOwMzNzEzW}            


## Notes and Errors:
None.

## References:
None.
