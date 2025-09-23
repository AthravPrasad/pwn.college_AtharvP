# Position Elsewhere   

## My Solve   
In this challenge when the terminal first opened we faced an issue to navigate to a directory that wasnt specified yet.    
So we just went forward ny hitting /challenge/run which told us the directory to run the path from.     
Once we got the path of the directory, we navigated using cd command and executed the file to get the flag.

*Flag* : pwn.college{w9HvCa3qu8VXyfSiVie4vN30E29.QX3QTN0wCOwMzNzEzW}

bash \
hacker@paths\~position-elsewhere:\~$ /challenge/run     
Incorrect...     
You are not currently in the /etc directory.    
Please use the `cd` utility to change directory appropriately.    
hacker@paths\~position-elsewhere:\~$ cd /etc    
hacker@paths\~position-elsewhere:/etc$ /challenge/run    
Correct!!!    
/challenge/run is an absolute path, invoked from the right directory!   
Here is your flag:    
pwn.college{w9HvCa3qu8VXyfSiVie4vN30E29.QX3QTN0wCOwMzNzEzW}    

## Notes:
No notes as such.

## References:
None.
