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



**CCA**



