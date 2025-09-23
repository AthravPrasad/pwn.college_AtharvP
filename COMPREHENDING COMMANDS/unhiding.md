## Unhiding Hidden Files

## My Solve:
Firstly list all hidden and unhidden files.
Then Using Cat Command Open the file most likely containing Flag.                   

*Flag:* pwn.college{kDD2nVLYzhQaaeonvrbGNnz8h7d.QXwUDO0wCOwMzNzEzW}                       

bash \
hacker@commands\~hidden-files:/$ ls -a                
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var                     
..  .flag-147772118713286  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr               
hacker@commands\~hidden-files:/$ cat  ./.flag-147772118713286                               
pwn.college{kDD2nVLYzhQaaeonvrbGNnz8h7d.QXwUDO0wCOwMzNzEzW}             

## Notes ANd Errors:
None.

## References:
None.
