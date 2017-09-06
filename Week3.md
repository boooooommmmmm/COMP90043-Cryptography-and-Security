# Week 3











### Block Cipher

Block Cipher: A block cipher takes a fixed length plain text message block (for example, 64 or 128 bits) and a key, and produces a cipher text block of the same length as the original message.

* Same key is used for many different message blocks.
* Diffusion dissipates statistical structure of plaintext over bulk of ciphertext.
* Confusion makes relationship between ciphertext and key as complex as possible.
* Generally diffusion is created by permutations and confusion is created by substitution.

### Stream Cipher

Stream Cipher: Takes a key of fixed size and generates a key stream in a pseudo random fashion with large period; this key stream is then combined with the plain text message stream on a bit by bit basis to form a cipher text stream.