# Filtering with grep -v

## My Solve:
The challenge required filtering out unnecessary output and displaying only the line containing the flag. 
I used the pipe operator (|) to direct the standard output (stdout) of /challenge/run into the grep command. I used the -v option with grep to invert the match, filtering out any lines that contained the word DECOY and successfully printing the flag.

*Flag:* pwn.college{UjlXo8oyF24YBiPjT-vW9aU98N7.0FOxEzNxwCOwMzNzEzW}

Bash

hacker@piping\~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY        
pwn.college{UjlXo8oyF24YBiPjT-vW9aU98N7.0FOxEzNxwCOwMzNzEzW}          
hacker@piping\~filtering-with-grep-v:~$           


## Notes and Errors: 
None.

## References:
None.
