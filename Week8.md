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



verify certificate, they can get public key.

---

END