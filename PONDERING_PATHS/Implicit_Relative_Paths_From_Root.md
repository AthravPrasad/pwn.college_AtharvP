# Implicit_Relative_Paths_From_Root

## My Solve:
This challenge was an upgraded version of the previous challenges.    
Here we had to first return to the root by the cd .. command .    
After that we had to invoke the challenge/run path to get the flag  

*Flag* : pwn.college{IZMJjHL2Ha8-1KE-MfqjrF7AeDM.QX5QTN0wCOwMzNzEzW}

bash \
hacker@paths/~implicit-relative-paths-from-:/~$ /challenge/run     
Incorrect...   
You are not currently in the / directory.   
Please use the `cd` utility to change directory appropriately.   
hacker@paths/~implicit-relative-paths-from-:/~$ cd ..    
hacker@paths/~implicit-relative-paths-from-:/home$ cd ..    
hacker@paths/~implicit-relative-paths-from-:/$ /challenge/run    
Incorrect...    
You invoked this challenge with an absolute path. This challenge needs a relative path!    
hacker@paths~implicit-relative-paths-from-:/$ challenge/run    
Correct!!!    
challenge/run is a relative path, invoked from the right directory!    
Here is your flag:    
pwn.college{IZMJjHL2Ha8-1KE-MfqjrF7AeDM.QX5QTN0wCOwMzNzEzW}    

## Notes and Errors:
Confused Absolute and relative directories, when i had to give the relative directory i accidentally entered the absolute one. 


## References:
None
