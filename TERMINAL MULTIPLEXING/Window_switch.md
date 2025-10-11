# Switching Windows


## My Solve:
The objective was to locate the flag hidden in a different terminal window within the current screen session.
The prompt indicated that the user was currently in "window 1" and that the flag was in "window 0".
The instructions explicitly stated to use the key combination Ctrl-A 0 to switch directly to the numbered window 0.

*Flag:* pwn.college{Yl_xOz2B3dtfiX8ABUxOSYg4dBO.0FO4IDOxwCOwMzNzEzW}

Bash

'''hacker@terminal-multiplexing\~switching-windows:\~$ cat <<MSG        
Welcome to the window switching challenge!          
You are currently in window 1.       
The flag is hidden in window 0.         
Use Ctrl-A 0 to switch to window 0!       
MSG       
Welcome to the window switching challenge!
You are currently in window 1.
The flag is hidden in window 0.
Use Ctrl-A 0 to switch to window 0!
hacker@terminal-multiplexing\~switching-windows:~$ cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{Yl_xOz2B3dtfiX8ABUxOSYg4dBO.0FO4IDOxwCOwMzNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{Yl_xOz2B3dtfiX8ABUxOSYg4dBO.0FO4IDOxwCOwMzNzEzW}
hacker@terminal-multiplexing\~switching-windows:\~$>


## Notes And Errors:
None.


## References:
None.
