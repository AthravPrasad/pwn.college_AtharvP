# Your First Shell Script

## My Solve:
The objective was to execute two commands, /challenge/pwn and /challenge/college, using a shell script.
I used the cat command with a here document (<<'EOF') to create the script file x.sh inline.
The here document redirected the commands to the file. Finally, I executed the script using bash x.sh, which ran the commands and retrieved the flag.

*Flag:* pwn.college{Eo9ZSSpfA48OTvjmy6wYJxiKPml.QXxcDO0wCOwMzNzEzW}

Bash

'''hacker@chaining\~your-first-shell-script:\~$ cat > x.sh <<'EOF'        
> /challenge/pwn            
> /challenge/college             
> EOF            
hacker@chaining\~your-first-shell-script:\~$ bash x.sh                    
Great job, you've written your first shell script! Here is the flag:                
pwn.college{Eo9ZSSpfA48OTvjmy6wYJxiKPml.QXxcDO0wCOwMzNzEzW}'''               


## Notes And Errors:
None.

## References:
None.
