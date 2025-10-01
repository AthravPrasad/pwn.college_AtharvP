# Process Substitution for Input

## My Solve:
I used the diff command with process substitution (<()) to compare the live output of /challenge/print_decoys and /challenge/print_decoys_and_flag, which extracted the flag line.

*Flag:* pwn.college{8bRMi_5t7X5jH4816DIH45joHWx.0lNwMDOxwCOwMzNzEzW}

Bash

'''hacker@piping\~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <( /challenge/print_decoys_and_flag)          
67a68           
pwn.college{8bRMi_5t7X5jH4816DIH45joHWx.0lNwMDOxwCOwMzNzEzW}              
hacker@piping\~process-substitution-for-input:~$    '''            
                    
## Notes and Errors:
None.

## References:
None.
