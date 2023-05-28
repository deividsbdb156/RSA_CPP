# RSA_CPP
RSA test code 
RSA algorithm is an asymmetric cryptography algorithm. Asymmetric actually means that it works on two different keys i.e. Public Key and Private Key. As the name describes that the Public Key is given to everyone and the Private key is kept private.


1: Creating Keys
•	Select two prime numbers x and y
•	Compute n = x * y where n is the modulus of private and the public key
•	Calculate totient function, ø (n) = (x − 1)(y − 1)
•	Choose an integer e such that e is coprime to ø(n) and 1 < e < ø(n). e is the public key exponent used for encryption
•	Now choose  d, so that d · e mod ø (n) = 1, ec, >code>d is the multiplicative inverse of e in mod ø (n)

2: Encrypting Message
•	Messages are encrypted using the Public key generated and is known to all.
•	The public key is the function of both e and n i.e. (e,n).
•	If M is the message(plain text), then ciphertext  C = M ^ n( mod n ) 

3: Decrypting Message
•	The private key is the function of both d and n i.e (d,n).
•	If C is the encrypted ciphertext, then the plain decrypted text M is M = C ^ d ( mod n)
