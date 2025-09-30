# Helpfull  Programs

## My Solve:
Firstly used --help program to find the next commands of what to do.
Then followed the commands and did as asked.


*Flag*:  pwn.college{Ezh4yje0X83ZErBgb7iXBl_mxYv.QX3IDO0wCOwMzNzEzW}              

bash \               
''' hacker@man~helpful-programs:~$ /challenge help                                               
bash: /challenge: Is a directory                        
hacker@man~helpful-programs:~$ /challenge --help           
bash: /challenge: Is a directory                
hacker@man~helpful-programs:~$ /challenge/challenge --help              
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]                

optional arguments:                
  -h, --help            show this help message and exit              
  --fortune             read your fortune                
  -v, --version         get the version number              
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG                    
                        get the flag, if given the correct value                              
  -p, --print-value     print the value that will cause the -g option to give you the flag              
hacker@man~helpful-programs:~$ /challenge/challenge -p             
The secret value is: 408                                          
hacker@man~helpful-programs:~$ /challenge/challenge --fortune             
Everyone talks about apathy, but no one does anything about it.               
hacker@man~helpful-programs:~$ /challenge/challenge -g                                       
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]                 
a challenge to make you ask for help: error: argument -g/--give-the-flag: expected one argument              
hacker@man~helpful-programs:~$ /challenge/challenge -g 408                               
Correct usage! Your flag: pwn.college{Ezh4yje0X83ZErBgb7iXBl_mxYv.QX3IDO0wCOwMzNzEzW}                 
hacker@man~helpful-programs:~$ '''                
                        
## Notes and Errors:           
Some Small Errors only.       

## References:         
None.     
