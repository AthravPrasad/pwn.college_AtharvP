# Deleting Newlines with tr

## My Solve:
The challenge output was split across multiple lines due to newline characters.
I used the tr command with the -d (delete) option to remove the newline character (\n). 

*Flag:* pwn.college{IOjkJ3oRxH2iSbIFfFTfetF_zFf.0VNxEzNxwCOwMzNzEzW}

Bash

'''hacker@data\~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{IOjkJ3oRxH2iSbIFfFTfetF_zFf.0VNxEzNxwCOwMzNzEzW}'''


## Notes and Errors:
None.

## References:
None.
