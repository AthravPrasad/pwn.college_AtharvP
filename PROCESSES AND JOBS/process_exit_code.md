# Process Exit Codes


## My Solve:
I executed the /challenge/get-code program. Immediately after its execution, I used the special shell variable $? to retrieve its exit code.
The exit code was determined to be 152. I then passed this code as an argument to the /challenge/submit-code program to retrieve the flag.

*Flag:* pwn.college{o_FIZp5PRfsbBrFhwFFhm1R8RT_.QX5YDO1wCOwMzNzEzW}

Bash

'''hacker@processes\~process-exit-codes:\~$ /challenge/get-code          
Exiting with an error code!         
hacker@processes\~process-exit-codes:\~$ echo $?              
152                  
hacker@processes\~process-exit-codes:\~$ /challenge/submit-code 152                   
CORRECT! Here is your flag:           
pwn.college{o_FIZp5PRfsbBrFhwFFhm1R8RT_.QX5YDO1wCOwMzNzEzW}              


## Notes and Errors:
None.

## References:
None.
