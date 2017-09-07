# Week 4



## Public Key





### Symmetric Key

DIS: 

* One key for en/de; 
* sender and receiver both need keep a key;
* One party can forge other party's data
* ​



### Asymmetric Key

* communication party are not equal
* two keys
* Non-Repudiation is possible.
* RSA/EIGamal/ECC based system

Encryption

Signatures: private key sign message, public key to verify message



### One way function

Computing f(x)=y given ‘x’ is easy

Given y=f(x), computing ‘x’ from ‘y’ is difficult or hard



### Discrete Logarithm Problem

离散对数问题

given g and h, hard to get x:

g^x = h 		<u>(mod p)</u>



### DH problem

Given g^ a and g^b, two arbitrary elements of the group G for some integers a and b in the range of 0 ≤a,b ≤ q, then find

​	g^(ab)

Normally G is a group in a suitable finite field.



### Diffie-Hellman

Alice and Bob share p and g (p=11, g=2)

g need to be primitive element 素元

Alice: g^n

Bob: g^m

g^n^m mod p = g^m^n mod p

**Problem:** 

cyclic group is finite field

man in middle

missing authentication



### Attack for RSA



**The basic RSA algorithm is vulnerable to CCA**

Attack

1. Compute X = (C x 2^e) mod n
2. Submit X as a chosen ciphertextand obtain corresponding plain text Y = X^dmod n.
3. Note that Y is in fact (2M) mod n
4. Compute M = Inverse(2) *Y mod n



CCA2



### Hard problems on RSA

1. Integer Factorization problem

2. RSA problem: 

   given e,c,n hard to find m

   m^e= c (mod n).