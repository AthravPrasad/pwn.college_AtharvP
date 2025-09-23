# Implicit Relative Path

## My Solve:
Firstly Navigate to the \challenge directory.
Here we have the run file from the current directory using a relative path so we specify it to linux, and run it using  <./run> and run it.

*Flag*: pwn.college{kyPpNVXndS7cp9EvjKcOTtbawN4.QXxUTN0wCOwMzNzEzW}    

bash   
hacker@paths\~implicit-relative-path:\~$ /challenge/run    
Incorrect...    
You are not currently in the /challenge directory.    
Please use the `cd` utility to change directory appropriately.    
hacker@paths\~implicit-relative-path:\~$ cd /challenge    
hacker@paths\~implicit-relative-path:/challenge$ ./run    
Correct!!!    
./run is a relative path, invoked from the right directory!    
Here is your flag:    
pwn.college{kyPpNVXndS7cp9EvjKcOTtbawN4.QXxUTN0wCOwMzNzEzW}    

## Notes and Errors:
None

## References:
None
