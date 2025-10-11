# Executable Shell Scripts


## My Solve:
The goal was to execute a command hidden within a shell script by granting the script executable permissions.
I used the cat command with a here document (<<'EOF') to quickly create a script file named run_challenge. The script contained the single command required to retrieve the flag: /challenge/solve.
I then used the chmod command with the symbolic mode (+x) to explicitly add execute permission to the run_challenge file.
Finally, I ran the script directly using its path (./run\_challenge), which successfully executed the internal command and revealed the flag.


*Flag:* pwn.college{IZ1dq4TegTNsFBFTxpaFojsjF9e.QX0cjM1wCOwMzNzEzW}

Bash

hacker@chaining\~executable-shell-scripts:\~$ cat > run_challenge <<'EOF'
> /challenge/solve
> EOF
hacker@chaining\~executable-shell-scripts:\~$ chmod +x run_challenge
hacker@chaining\~executable-shell-scripts:\~$ ./run_challenge
Congratulations on your shell script execution! Your flag:
pwn.college{IZ1dq4TegTNsFBFTxpaFojsjF9e.QX0cjM1wCOwMzNzEzW}


## Notes And Errors:
None.

## References:
None.







