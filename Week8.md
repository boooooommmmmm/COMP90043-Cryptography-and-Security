# Week 8

This week is talking about public key and ElGamal

### Distribution of Public Keys

* public announcement
* publicly available directory
* public-key authority
* public-key certificates

Last two are efficacy in the Internet.



Signature is using private function for hashed message.

Verification is using the same encryption algorithm with public key.



#### Public Announcement

* broadcast
* weakness is forgery

<br />

#### Publicly Available Directory

* Maintenance and distribution of the public directory would have to be the responsibility of some trusted entity or organization.
* The authority maintains a directory with a {name, public key} entry for each participant.
* Vulnerabilities:  computing the private key of the directory authority.

<br />

#### Public-Key Authority

* requires users to know public key for the directory
* More stable
* Need to be on-line at all time

<br />

#### Public-Key Certificates

* a certificate binds identity to public key
* signed by CA (**Certificate Authority**)

<br />

#### CA Hierarchy

* each CA has certificates for clients (forward) and parent (backward)

<br />

#### Certificate Revoke

<br />

1. Each certificate includes a period of validity
2. Can be revoke before it expries.
3. Each CA must maintain a list consisting of all revoked but not expired certificates issued by that CA



##### Three extensions of X.509 Version 3

1. Key and policy information
2. Subject and issure attributes
3. Certification path constraints


<br />


##### PKIX（public key infrastructure）

PKIX identifies a number of management functions that potentially need to be supported by management protocols:

<br />

verify certificate, they can get public key.

<br />

<br />

## ElGamal Cryptography

Related to Diffie-Hellman problem

* difficulty of computing discrete logarithms, as in D-H
* difficulty of computational D-H problem.



---

END