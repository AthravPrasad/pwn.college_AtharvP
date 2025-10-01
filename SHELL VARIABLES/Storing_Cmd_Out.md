# Storing Command Output

## My Solve:
I executed the /challenge/run program and stored its entire standard output (stdout) directly into the environment variable PWN using command substitution (the syntax $(...)). 
I then printed the contents of the variable using echo $PWN to reveal the flag.

*Flag:* pwn.college{Iik70zZCAKdq_PI8mzEqQpB5_KY.QX1cDN1wCOwMzNzEzW}

Bash

hacker@variables\~storing-command-output:~$ PWN=$( /challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables\~storing-command-output:~$ echo $PWN
pwn.college{Iik70zZCAKdq_PI8mzEqQpB5_KY.QX1cDN1wCOwMzNzEzW}


## Notes and Errors:
None.

## References:
None.







