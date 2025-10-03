# Sorting Data and Extracting the Top Line

## My Solve:
I used the sort command to process the contents of /challenge/flags.txt. 
I applied the -r (reverse) option to sort the lines in descending order (Z to A). 
I then piped the output into the head -n 1 command to extract the very first line of the sorted list, which contained the flag.

*Flag:* pwn.college{MxFgKosI_ClgiZZtKbMki5vV4Y8.0FM0MDOxwCOwMzNzEzW}

Bash

'''hacker@data\~sorting-data:~$ sort -r /challenge/flags.txt | head -n 1
pwn.college{MxFgKosI_ClgiZZtKbMki5vV4Y8.0FM0MDOxwCOwMzNzEzW}'''

## Notes and Errors:
None.

## References:
None.
