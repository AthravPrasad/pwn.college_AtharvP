# Deleting Characters with tr


## My Solve:
I used the tr command with the -d (delete) option to remove the extraneous characters from the output.
Did it and got the flag.

*Flag:* pwn.college{sSPH9jKLrzzgow8efneASUp2tnb.0FNxEzNxwCOwMzNzEzW}

Bash

'''hacker@data\~deleting-characters:~$ /challenge/run | tr -d ^%        
Your character-stuffed flag:            
pwn.college{sSPH9jKLrzzgow8efneASUp2tnb.0FNxEzNxwCOwMzNzEzW}'''                      

## Notes and Errors:
None.

## References:
None.
