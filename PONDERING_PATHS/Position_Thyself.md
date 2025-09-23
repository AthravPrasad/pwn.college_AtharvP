# Position Thyself   

## My Solve   
In this challenge when the terminal first opened we faced an issue to navigate to a directory that wasnt specified yet.    
So we just went forward ny hitting /challenge/run which told us the directory to run the path from.     
Once we got the path of the directory, we navigated using cd command and executed the file to get the flag.

*Flag* : pwn.college{k0y_HNA7Kgpx4QswF9zKmW-Xz6e.QX2QTN0wCOwMzNzEzW}

bash \
hacker@paths/~position-thy-self:/~$ /challenge/run  
Incorrect...   
You are not currently in the /usr/include directory.    
Please use the `cd` utility to change directory appropriately.    
hacker@paths/~position-thy-self:/~$ cd /usr/include    
hacker@paths/~position-thy-self:/usr/include$ /challenge/run    
Correct!!!    
/challenge/run is an absolute path, invoked from the right directory!    
Here is your flag:    
pwn.college{k0y_HNA7Kgpx4QswF9zKmW-Xz6e.QX2QTN0wCOwMzNzEzW}    

## Notes:
No notes as such.

## References:
None.


