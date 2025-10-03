# Extracting Specific Sections of Text with cut


## My Solve:
I set the delimiter to a space (-d " ") and selected the second field (-f 2), which contained the actual flag string. 
Since the output was newline-separated, I then piped the result to tr -d "\n" to remove all newline characters, concatenating the parts into the final flag.

*Flag:* pwn.college{UKCn6D61313aa2gAMKdtqH0vRO1.01NxEzNxwCOwMzNzEzW}

Bash

'''hacker@data\~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{UKCn6D61313aa2gAMKdtqH0vRO1.01NxEzNxwCOwMzNzEzW}'''

## Notes and Errors:
None.

## References:
None.##
