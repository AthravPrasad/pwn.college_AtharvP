# Explicit Relative Path from Root

## My Solve:
This problem was similar to the previous one where we had to navigate to root first, then invoke the  challenge/run file from there.
The additional Feature here was that we had to use <.> .

*Flag* : pwn.college{wIwawx0DTKDXP52ySunNVuQFP_p.QXwUTN0wCOwMzNzEzW}

bash \
hacker@paths\~explicit-relative-paths-from-:\~$ /challenge/run   
Incorrect...   
You are not currently in the / directory.    
Please use the `cd` utility to change directory appropriately.    
hacker@paths\~explicit-relative-paths-from-:\~$ cd ..    
hacker@paths\~explicit-relative-paths-from-:/home$ cd ..    
hacker@paths\~explicit-relative-paths-from-:/$ .challenge/run    
bash: .challenge/run: No such file or directory    
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run    
Correct!!!    
./challenge/run is a relative path, invoked from the right directory!    
Here is your flag:     
pwn.college{wIwawx0DTKDXP52ySunNVuQFP_p.QXwUTN0wCOwMzNzEzW}   

## Notes and Errors:
Mistakenly missed the / after . ( more of a typo honestly).

## References:   
None.
 
