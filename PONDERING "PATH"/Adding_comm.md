# Adding Commands to PATH


## My Solve:
The objective was to trick the /challenge/run program into executing a user-defined command named win to read the flag. This was accomplished by creating a custom directory, placing an executable file named win inside it, and adding the directory to the system's execution path.
Create Custom Directory: Used mkdir -p "$HOME/mybin" to create a private directory for custom executables.
Create Custom Command: Used cat with a here document (<<'SH') to create an executable file named win inside the new directory. The content of this file was simply /bin/cat /flag.
Set Permissions: Used chmod +x "$HOME/mybin/win" to make the new script executable.
Modify PATH: Set the PATH environment variable to exclusively include the new directory: PATH="$HOME/mybin".
Execute: When /challenge/run executed, it attempted to find win in the new, customized PATH, found our script, ran it, and output the flag.

*Flag:* pwn.college{YGoIpjROVvbthQ1AkjwYQI8PQ6O.QX2cjM1wCOwMzNzEzW}

Bash

'''hacker@path\~adding-commands:\~$ mkdir -p "$HOME/mybin"
hacker@path\~adding-commands:\~$ cat > "$HOME/mybin/win" <<'SH'
> /bin/cat /flag
> SH
hacker@path\~adding-commands:\~$ chmod +x "$HOME/mybin/win"
hacker@path\~adding-commands:\~$ PATH="$HOME/mybin"
hacker@path\~adding-commands:\~$ /challenge/run
Invoking 'win'....
pwn.college{YGoIpjROVvbthQ1AkjwYQI8PQ6O.QX2cjM1wCOwMzNzEzW}'''


## Notes And Errors:
None.

## References:
None.







