## Help For Builtins

## My Solve:
Firstly Accessed the the shell builtin after which, we took the commands given therre to get the flag

*FLAG:*pwn.college{AbsefYRHnYZA3csn94xBUWVJImR.QX0ETO0wCOwMzNzEzW}

bash \
''' hacker@man~help-for-builtins:/challenge$ help challenge       
challenge: challenge [--fortune] [--version] [--secret SECRET]                   
    This builtin command will read you the flag, given the right arguments!                  
    
    Options:                                
      --fortune         display a fortune            
      --version         display the version                   
      --secret VALUE    prints the flag, if VALUE is correct             
 
    You must be sure to provide the right value to --secret. That value            
    is "AbsefYRH".                                        
hacker@man~help-for-builtins:/challenge$ ls /challenge          
DESCRIPTION.md                    
hacker@man~help-for-builtins:/challenge$ challenge --secret AbsefYRH          
Correct! Here is your flag!            
pwn.college{AbsefYRHnYZA3csn94xBUWVJImR.QX0ETO0wCOwMzNzEzW} '''        

## Notes and Errors:
None.

## References:
NOne.
