## Matching With []

## My Solve:
Changed the directory and found the flag by searching for the file using [].

*Flag:* pwn.college{4l7zDzPHUGvGJnofO-5Z4sw1Wg5.QXzIDO0wCOwMzNzEzW}

bash \
''' hacker@globbing~matching-with-:~$ cd /c*/fil*                
hacker@globbing~matching-with-:/challenge/files$ /ch*/r* file[bash]                 
Your expansion did not expand to the requested files (file_a, file_b, file_h,                    
and file_s). Instead, it expanded to:                  
file[bash]                    
hacker@globbing~matching-with-:/challenge/files$ /ch*/r* file_[bash]              
You got it! Here is your flag!               
pwn.college{4l7zDzPHUGvGJnofO-5Z4sw1Wg5.QXzIDO0wCOwMzNzEzW} '''         

## Notes And Errors:
Missed a _.

## References:
None.


