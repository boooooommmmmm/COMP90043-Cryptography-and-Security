# Week2
This week is talking about symmetric key cryptography

<br/>

## Euclid's algorithm
Let a, b, q, r be integers with such that a = qb + r . Then gcd(a, b) = gcd(b, r ).<br />
gcd(33, 21)
33 = 1 * 21 + 12 gcd(21, 12)
21 = 1 * 12 + 9 gcd(12, 9)
12 = 1 * 9 + 3 gcd(9, 3)
9 = 3 * 3 + 0 gcd(3, 0)
Table: Determination of gcd(33, 21)<br />

## Modular Multiplicative Inverse
X 圈乘n y = 1;
then we say y is the **multiplicative inverse** of x. It is denoted by y = x^(-1) usually. <br />

## Determining multiplicative inverse
gcd[a, b] := ax + by:
gcd(a, n) = 1.

## Extend Euclid's algorithm
gcd(a, b) = at = x a + y b;<br />
If gcd(n, a) is 1; xn + ya = 1. -> ya = 1 mod n.

<hr >
<br/>

## Symmetric Encryption
* Main assumption: Sender and recipient share a common key 
* All classical encryption algorithms are private-key
* far most widely used

<br/>

### key words

**plaintext** - original message

**ciphertext** - coded message

**cipher** - algorithm for transforming plaintext to ciphertext

**key** -info used in cipher known only to sender/receiver; required for en/de algorithm

**encipher (encrypt)** - converting plaintext to ciphertext

**decipher (decrypt)** - recovering plaintext from ciphertext

**cryptography** - study of encryption principles/methods -> 密码学

**cryptanalysis (code breaking)** - study of principles/ methods of deciphering ciphertext without knowing key -> 密码分析 ->Objective to recover key, not just message ->cryptanalytic attack/cryptanalytic attack

**cryptology** - field of both cryptography and cryptanalysis
<br/>

<br />

### *Two requirements for secure use of symmetric encryption*

* a strong encryption algorithm

* a secret key is known only to sender/receiver

<br/>

#### Type of encryption operations used

1. Substitution
2. Transposition
3. Product

<br/>

#### General approaches

* cryptanalytic attack
* brute-force attack

**cryptanalysis (code breaking)** - study of principles/ methods of deciphering ciphertext without knowing key -> 密码分析 ->**Objective to recover key, not just message** ->cryptanalytic attack/cryptanalytic attack

<br/>
<br/>

### Cryptanalytic Attacks

ciphertext only - only know algorithm & ciphertext, is statistical, know or can identify plaintext -> still need guess in sometimes

known plaintext - know/suspect plaintext & ciphertext

chosen plaintext - select plaintext and obtain ciphertext

chosen ciphertext

chosen text - select plaintext or ciphertext to en/decrypt

<br/>
<br/>

### unconditional security/conditional security 

-> 无条件安全，有条件安全

-> no matter how much computer power or time is available

-> given limited computing resources (eg time needed for calculations is greater than age of universe)

<br/>
<br/>

## Cipher methods

* Classical **Substitution** Ciphers -> 代换加密 -> change letters with other numbers or symbols

  * Caesar Cipher - replaces each letter by 3rd letter on - earliest - c = E(p) = (p + k) mod (26)

  * Monoalphabetic Cipher -> 表单密码 -> each plaintext letter maps to a different random ciphertext letter -> hence key is 26 letters long -> 26! keys -> can use Language Redundancy and Cryptanalysis
* Polyalphabetic Ciphers -> 多表单替换密码 -> Improve security using multiple cipher alphabets -> Use a key to select which alphabet is used for each letter of the message -> repeat from start after end of key is reached
  * Vigenère Cipher -> 维吉尼亚密码 -> Polyalphabetic Ciphers -> hence letter frequencies are obscured, but not totally lost
* One-Time Pad -> 单次密本 -> if a truly random key as long as the message is used, the cipher will be secure called a One-Time pad -> is unbreakable since ciphertext bears no statistical relationship to the plaintext -> since for any plaintext& any ciphertextthere exists a key mapping one to other -> only use once -> problems in generation & safe distribution of key
* Transposition cipher -> 转置密码 -> rearranging the letter order -> can recognise these since have the same frequency distribution as the original text
  * Rail Fence cipher -> 栅栏加密法 -> write message letters out diagonally over a number of rows
  * Row Transposition Ciphers -> write letters of message out in rows over a specified number of columns -> then reorder the columns according to some key before reading off the rows
* Product Ciphers -> ciphers using substitutions or transpositions are not secure because of language characteristics -> Rotor Machines
* Steganography -> 速记式加密 -> using invisible ink


***

#### Language Redundancy and Cryptanalysis:

human languages are redundant

letters are not equally commonly used

in English, E is by far the most common letter

other letters like Z,J,K,Q,X are fairly rare

English Letter Frequencies



#### Kasiski Method




















