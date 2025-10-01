# Matching with *

## My Solve:
I needed to use a single glob pattern to expand to the files containing the letter 'p' anywhere in their name: happy, optimistic, and splendid.
The pattern *p* successfully matched all required files and provided the flag.

*Flag*: pwn.college{sDwLIFWAfnSbiN82o2LB_lBFaoL.0lM3kjNxwCOwMzNzEzW}

bash \
hacker@globbing\~multiple-globs:\~$ cd /challenge/files                  
hacker@globbing\~multiple-globs:/challenge/files$ /challenge/run p**                       
Your expansion did not expand to the requested files (happy optimistic pwning splendid uplifting).         
Instead, it expanded to:                        
pwning                        
hacker@globbing\~multiple-globs:/challenge/files$ /challenge/run *p*             
You got it! Here is your flag!                
pwn.college{sDwLIFWAfnSbiN82o2LB_lBFaoL.0lM3kjNxwCOwMzNzEzW}           
hacker@globbing\~multiple-globs:/challenge/files$              

## Notes and Errors:
My initial attempt with p** only matched files starting with 'p'. The correct glob was *p* to match the letter 'p' at any position.

## References:
None.
