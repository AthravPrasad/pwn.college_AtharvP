# Named Pipes (FIFOs)

## My Solve:
Used **`mkfifo`** to create a **named pipe (`/tmp/flag_fifo`)**. Then, initiated a background process (`&`) using **`cat`** to open the read side of the pipe, causing it to block. Finally, executed `/challenge/run` and redirected its output to the write side of the pipe (`> /tmp/flag_fifo`), unblocking the process and capturing the flag.

*Flag:* pwn.college{AE-frFDb2yo7ebHmUeyKdyeFL0j.01MzMDOxwCOwMzNzEzW}

bash

'''hacker@piping\~named-pipes:~$ mkfifo /tmp/flag_fifo     
hacker@piping\~named-pipes:~$ cat /tmp/flag_fifo &             
[1] 149       
hacker@piping\~named-pipes:~$ /challenge/run > /tmp/flag_fifo          
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!         
Bash will now try to open the FIFO for writing, to pass it as the stdout of            
/challenge/run. Recall that operations on FIFOs will *block* until both the           
read side and the write side is open, so /challenge/run will not actually be          
launched until you start reading from the FIFO!                    
You've correctly redirected /challenge/run's stdout to a FIFO at           
/tmp/flag_fifo! Here is your flag:            
pwn.college{AE-frFDb2yo7ebHmUeyKdyeFL0j.01MzMDOxwCOwMzNzEzW}         
[1]+  Done                    cat /tmp/flag_fifo             


## Notes and Errors:
None.

## References:
None.

