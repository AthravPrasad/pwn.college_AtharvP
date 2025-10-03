# Translating Characters with tr

## My Solve:
I used the tr (translate) command, piping the challenge output directly to it. 
I defined the source set as all lowercase letters followed by all uppercase letters, and the target set as all uppercase letters followed by all lowercase letters. 

*Flag:* pwn.college{sjVaiXmanD4Ycj0lIVRI-f_5lKD.01MxEzNxwCOwMzNzEzW}

Bash

''' hacker@data\~translating-characters:\~$ /challenge/run        
Your case-swapped flag:          
PWN.COLLEGE{SJvAIxMANd4yCJ0Livri-F_5Lkd.01mXeZnXWcoWmZnZeZw}             

hacker@data\~translating-characters:~$ /challenge/run | tr abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz                
yOUR CASE-SWAPPED FLAG:             
pwn.college{sjVaiXmanD4Ycj0lIVRI-f_5lKD.01MxEzNxwCOwMzNzEzW} '''           


## Notes and Errors:
None.

## References:
None.
