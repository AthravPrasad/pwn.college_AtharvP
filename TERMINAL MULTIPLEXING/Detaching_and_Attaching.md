# Detaching and Attaching (tmux)


## My Solve
Used the tmux command to create a new session, detached using the keyboard prefix (Ctrl+B, D), ran the challenge program. T
hen used tmux attach to re-enter the session and retrieve the flag.

*Flag:* pwn.college{8CNlIg78YoWjKh6JK8cDhjCRHmf.0VO4IDOxwCOwMzNzEzW}

Bash

'''hacker@terminal-multiplexing\~detaching-and-attaching-tmux:\~$ tmux         
\[detached (from session 0)]          
hacker@terminal-multiplexing\~detaching-and-attaching-tmux:\~$ /challenge/run        
Found detached tmux session: 0          
Sending flag to your tmux session...        

Flag sent! Now reattach to your tmux session with:       
  tmux attach     
hacker@terminal-multiplexing\~detaching-and-attaching-tmux:\~$ tmux attach      
hacker@terminal-multiplexing\~detaching-and-attaching-tmux:\~$       
echo Congratulations, here is your flag: pwn.college{8CNlIg78YoWjKh6JK8cDhjCRHmf.0VO4IDOxwCOwMzNzEzW}        
Congratulations, here is your flag: pwn.college{8CNlIg78YoWjKh6JK8cDhjCRHmf.0VO4IDOxwCOwMzNzEzW}'''           


## Notes And Errors:
None.

## References:
None.
