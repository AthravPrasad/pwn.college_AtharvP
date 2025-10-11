# Detaching and Attaching a Screen Session


## My Solve:
The objective was to start a terminal session in the background, detach from it, run a challenge program that communicates with that session, and then reattach to retrieve the flag. This tests the basic workflow of the screen utility.
I manually printed a placeholder flag first.
I started a new screen session by simply running screen.
I immediately detached the active screen session by pressing the keyboard shortcut Ctrl+A followed by D.
I ran the checker program, /challenge/run, which detected the detached session and sent the flag to it.
I reattached to the session using the command screen -r to view the waiting flag output.


*Flag:* pwn.college{4vRUN8ymtg_XF6iGBxSzrcMgyiP.0lN4IDOxwCOwMzNzEzW}

Bash

hacker@terminal-multiplexing\~detaching-and-attaching:\~$ echo Yes! Flag is: pwn.college{4vRUN8ymtg_XF6iGBxSzrcMgyiP.0lN4IDOxwCOwMzNzEzW}         
Yes! Flag is: pwn.college{4vRUN8ymtg_XF6iGBxSzrcMgyiP.0lN4IDOxwCOwMzNzEzW}hacker@terminal-multiplexing\~detaching-and-attaching:~$ screen            
\[detached from 147.pts-0.terminal-multiplexing~detaching-and-attaching]             
hacker@terminal-multiplexing\~detaching-and-attaching:\~$ /challenge/run                  
Found detached screen session: 147.pts-0.terminal-multiplexing\~detaching-and-attaching          
Sending flag to your screen session...               

Flag sent! Now reattach to your screen session with:

 screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing\~detaching-and-attaching:\~$ screen -r
\[screen is terminating]


## Notes And Errors:
None.

## References:
None.
