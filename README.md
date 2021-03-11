# Caesar Cipher
The encryption can be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A = 0, B = 1,…, Z = 25. Encryption of a letter by a shift n can be described mathematically as.
Algorithm for Caesar Cipher:
Input:

A String of lower case letters, called Text.
An Integer between 0-25 denoting the required shift.
Procedure:

1.Traverse the given text one character at a time .
2.For each character, transform the given character as per the rule, depending on whether we’re encrypting or decrypting the text.
3.Return the new string generated.
4.Program that receives a Text (string) and Shift value( integer) and returns the encrypted text.

How to decrypt?
We can either write another function decrypt similar to encrypt, that’ll apply the given shift in the opposite direction to decrypt the original text. However we can use the cyclic property of the cipher under modulo , hence we can simply observe

Cipher(n) = De-cipher(26-n)
Hence, we can use the same function to decrypt, instead we’ll modify the shift value such that shift = 26-shift 
