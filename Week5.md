# Week 5



## RSA Signatures

* Signature is a pattern that depends on the message being singend
* Must use some information unique to the sender to prevent both forgery and denial
* Relatively easy to produce the digital signature
* Relatively easy to recognize and verify the digital signature
* Computationally infeasible to forge a digital signature



### RSA Signatures properties 

* RSA signature is a public key signature scheme
* Signature is a means for a trusted third party to bind the identity of a user to a public key
* Complement of RSA public encryption
* Private key signs messages; public key verify the signatures



### Forgery attack

s = M^d mod N

(M1 * M2)^d= M1^d* M2^d

(s1 * s2) is the signature of (M1*M2).



### Blinding

Alice’s public key – [N,e]; Private key [d]

Choose a random x – in the range [0..N-1]

Form a blinded message -- Mb = x ^ e * M mod N

Alice may sign sb = Mb^d mod N

**s = sb/x mod N**

s^ e = sb^e /x ^e = (Mb)^d e /x^ e = (Mb) /x^ e = x^ e M / x^ e = M

Hence s is the signature of M.