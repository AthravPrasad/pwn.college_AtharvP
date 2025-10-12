My solve...
The command injection vulnerability is exploited by figuring out that the URL-encoded newline character, %0A, can be effectively utilized to chain multiple shell commands together.
Initial directory reconnaissance is performed using the ls command to list available files. The contents of the mission_briefing.txt file are then read using the less command, which reveals a hint about the key's location being deep within the AetherCorp network.
Subsequent searches focus on the standard library directories.
The aethercorp directory is located within /var/lib/, and navigation to this path is executed.
Further use of ls within this new directory identifies an archive subdirectory.
A hidden directory, .secrets, is then discovered inside the archive using the ls /var/lib/aethercorp/archive -a command.
Finally, listing the contents of the hidden directory with ls /var/lib/aethercorp/archive/.secrets reveals the target file, blacksite_key.dat.
The flag is successfully extracted by reading the contents of this file using the final command: less /var/lib/aethercorp/archive/.secrets/blacksite_key.dat. 

*Flag:* citadel{bl4ck51t3_4cc3ss_gr4nt3d}
