# Mixing Globs

## My Solve:
The challenge required using a square bracket glob ([]) to match the three required files.
I observed that these three files are the only ones that start with one of the characters 'c', 'e', or 'p'.
The glob pattern [cep]* matched any file starting with 'c', 'e', or 'p',, successfully yielding the flag.

*Flag:* pwn.college{8KmgqNF90Q1MXPyRO0_er_CJoCU.QX1IDO0wCOwMzNzEzW}

Bash

hacker@globbing\~mixing-globs:\~$ cd /challenge/files         
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run *ing*            
Error: you did not use a square bracket glob...                     
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*              
You got it! Here is your flag!             
pwn.college{8KmgqNF90Q1MXPyRO0_er_CJoCU.QX1IDO0wCOwMzNzEzW}          
hacker@globbing~mixing-globs:/challenge/files$           
Notes and Errors:             
The first attempt, *ing*, failed because it used only the asterisk wildcard and did not include the required square bracket glob ([]).             

## References:
None.

## Notes and Errors:
The first attempt, *ing*, failed because it used only the asterisk wildcard and did not include the required square bracket glob ([]).










