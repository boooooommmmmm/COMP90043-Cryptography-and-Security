# Week 10

<br />

## User Authentication

user authentication is the fundamental building block and the primary line of defense. 

User authentication is the basis for most types of access control and for user accountability

Identificaiton -> specify identifier

Verification -> bind entity and identifier

<br />

### Means of user Authentication

1. Something the individual knows -> password, PIN
2. Something the individual possesses -> cryptographic keys, token
3. Something the individual is static biometrics -> fingerprint, face which consider as unique.
4. Something the individual is dynamic biometrics -> voice pattern, handwriting characteristics, and typing rhythm.

<be />

### Mutual Authentication

Protocols enables mutually change identify and session key

**Two issues:** 

1. confidentiality
2. Timeliness

<br />

### Replay Attack

1. send message latter
2. replay time-stamped message within the valid time.
3. Opponent suppresses the original message. Thus, the repetition cannot be detected.
4. Backward replay without modification. ->replay back to the message sender (symmetric encryption).

Approach:

1. sequence number
2. Timestamps
3. challenge/response

<br />

### One-way Authentication

Email

### Needham-Schroeder Protocol

Vulnerable to a replay attack if an old session key has been compromised



### Suppress-Replay Attacks

For Denning 81 modification protocol

When sender's clock is ahead of the intended recipient's clock.





## Kerberos

Kerberos is an authentication server developed as a part Project Athena.

workstations can access services on servers distributed throughout the network

servers to be able to restrict access to authorized users and to be able to authenticate requests for service

#### Requirement:

1. Secure
2. Reliable -> distribution server architecture and back up. 
3. Scalable
4. Transparent -> user should not be aware authentication is taking place.



AS

TS

TGS





---

END

