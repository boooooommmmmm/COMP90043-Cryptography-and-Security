# Week 7

<br />

---

Middle exam this week, no second lecture.

---

<br />

## Key Distribution

Use common security key.

Main purpose of key distribution to ensure that keys are private between the sender and receiver.

Need frequency changing the keys. -> limits the ability of ...



**Key distribution alternatives**

1. physically deliver
2. third part **select or deliver key**.
3. using previous key to encrypt a new key
4. third party C to **relay key** if the communications channels with C are secured


<br />


### Key Hierarchy

**Session key**

A temporary key

For one logical session only



**Master key**

For encrypt session key

Shared by user and key distribution centre.



`However, the scale of the problem is vastly reduced, as only N master keys are required, one for each entity. Thus, master keys can be distributed in some non-cryptographic way, such as physical delivery. `



### Key Distribution Scenario

Assumption: 

1. A wants to communicates with B.
2. Each user have master key agreed with KDC.

![w7_1](.\PIC\w7_1.png)

**Issues**

* If two entities in different domains desire a shared key, then the corresponding local KDC’s can communicate through a global KDC
* The hierarchical concept can be extended to three or more layers
* Scheme minimizes the effort involved in master key distribution because most master keys are those shared by a local KDC with its local entities



### Hybrid Key Distribution

* retain use of private-key KDC
* shares secret master key with each user
* distributes session key using master key
* public-key used to distribute master keys
  * especially useful with widely distributed users
* rationale
  * performance
  * backward compatibility





### Random Numbers

statistically random, uniform distribution, independent

unpredictability of future values from previous values



**Pseudorandom Number Generators (PRNGs)**

not truly random

can pass random test



**Linear Congruential Generator**

Xn+1= (aXn+ c) mod m



**Using Block Ciphers as PRNGs**



**Blum Blum Shub Generator**

xi= (x(i-1)) ^ 2mod n
where n=p.q, and primes p,q=3 mod 4

Unpredictable

difficulty of factoring n

slow



**Natural Random Noise**

Find a regular but random event and monitor

Problems for bias or uneven distribution and use



**Published Sources**





<br />

---

END