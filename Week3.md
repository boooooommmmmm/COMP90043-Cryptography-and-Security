# Week 3

### One Time Pad

* Random secret key
* Unconditional Security
* The adversary will not learn any knowledge to reverse the encryption from watching cipher text even with unlimited computing power.
* Seeing the cipher text C does not increase the adversaries knowledge about the message.



<br />

<br />

### Block Cipher

Block Cipher: A block cipher takes a **fixed length** plain text message block (for example, 64 or 128 bits) and a key, and produces a cipher text block of the same length as the original message.

* Same key is used for many different message blocks.
* Diffusion dissipates statistical structure of plaintext over bulk of ciphertext.
* Confusion makes relationship between ciphertext and key as complex as possible.
* Generally diffusion is created by permutations and confusion is created by substitution.

### Stream Cipher

Stream Cipher: Takes a key of fixed size and generates a key stream in a pseudo random fashion with large period; this key stream is then combined with the plain text message stream on a bit by bit basis to form a cipher text stream.







### Electronic Codebook Book (ECB)

* message is broken into independent blocks which are encrypted

* each block is a value which is substituted, like a codebook, hence name

* each block is encoded independently of the other blocks

  ​	Ci= EK(Pi)

* uses: secure transmission of single values

Limitations

* message repetitions may show in ciphertext
  * p1=p2;c1=c2
  * messages that change very little



### Cipher Block Chaining (CBC)

* message is broken into blocks
* linked together in encryption operation
* use Initial Vector (IV) to start process
  Ci= EK (Pi  XOR Ci-1)
  C-1= IV



### Message Padding

* at end of message must handle a possible last short block
  * not as large as blocksize of cipher
  * pad either with known non-data value
  * pad last block along with count of pad size
  * may require an extra entire block over those in message





### Output FeedBack (OFB)

* message is treated as a stream of bits
* output of cipher is added to message
* output is then feed back (hence name)
* feedback is independent of message
* can be computed in advance
  Oi= EK(Oi-1)
  Ci= PiXOR Oi
  O-1= IV
* uses: stream encryption on noisy channels
* ==================
* needs an IV which is unique for each use
* bit errors do not propagate
* more vulnerable to message stream modification
* sender & receiver must remain in sync
* only use with full block feedback