# Command Chaining with Logical OR (||)

## My Solve:
This challenge required executing /challenge/second only if the previous command, /challenge/first-failure, failed. 
I used the conditional OR operator (||) for this error handling chain. The first command failed (as designed), allowing the second command to run and retrieve the flag.

*Flag:* pwn.college{g1xOWkq1LLyMNiQiTj1gQNAVUPT.01MOMDOxwCOwMzNzEzW}

Bash

hacker@chaining\~handling-failure:~$ /challenge/first-failure || /challenge/second       
Nice chaining! Flag: pwn.college{g1xOWkq1LLyMNiQiTj1gQNAVUPT.01MOMDOxwCOwMzNzEzW}             

## Notes And Errors:
None.

## References:
None.

