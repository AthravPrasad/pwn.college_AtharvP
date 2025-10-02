# Writing to Multiple Programs

## My Solve:
Used **`tee`** with **process substitution (`>()`)** to pipe the output of `/challenge/hack` to both `/challenge/the` and `/challenge/planet` simultaneously.

*Flag:* pwn.college{wwfBUhokW9aqqJeHk3renmdH26A.QXwgDN1wCOwMzNzEzW}**

bash

'''hacker@piping\~writing-to-multiple-programs:\~$ /challenge/hack | tee >( /challenge/the ) >( /challenge/planet )            
This secret data must directly and simultaneously make it to /challenge/the and             
/challenge/planet. Don't try to copy-paste it; it changes too fast.             
1251431021255920991                                
Congratulations, you have duplicated data into the input of two programs! Here              
is your flag:       
pwn.college{wwfBUhokW9aqqJeHk3renmdH26A.QXwgDN1wCOwMzNzEzW}'''           

## Notes and Errors:
None.

## References:
None.
