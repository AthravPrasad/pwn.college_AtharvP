# Making Files Executable

## My Solve:
The target binary, /challenge/run, initially lacked the executable permission.
I used the chmod command to add the executable bit (+x) for the user. 
Once the permission was modified, running the file executed the program successfully and revealed the flag.

*Flag:* pwn.college{AHy0b-Ok_wWtPStuCq1ebalnJDf.QXyEjN0wCOwMzNzEzW}

Bash

hacker@permissions\~executable-files:~$ chmod +x /challenge/run     
hacker@permissions\~executable-files:~$ /challenge/run                
Successful execution! Here is your flag:                      
pwn.college{AHy0b-Ok_wWtPStuCq1ebalnJDf.QXyEjN0wCOwMzNzEzW}                
hacker@permissions\~executable-files:~$          


## Notes And Errors:
None.

## References:
None.

