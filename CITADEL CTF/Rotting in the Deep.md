# My solve
The flag was initially converted into an integer, and subsequently, every individual digit within that integer was subjected to a positive shift of 3. 
The provided Python script precisely implements the reversal of this shifting process.
It iterates through the string of ciphertext digits (ct), converts each character to an integer, subtracts 3 from it, and then applies the modulo 10 operation to correctly handle negative results (effectively an un-shift or ROT-3 decode on each digit).
The resulting string of un-shifted digits is then converted back to a large integer, which is finally transformed into its corresponding byte string to reveal the plaintext flag.
This successful reversal yields the final secret message. 

*flag:* citadel{br0_r34lly_unr0tt3d_m3_b4ck_t0_l1f3}
