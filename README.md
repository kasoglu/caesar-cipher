# Caesar Cipher Encryption&Decryption
# History

The Caesar cipher is named after Julius Caesar, who, according to Suetonius, used it with a shift of three (A becoming D when encrypting, and D becoming A when decrypting) to protect messages of military significance. While Caesar's was the first recorded use of this scheme, other substitution ciphers are known to have been used earlier.

# Usage
![caesar_cipher](https://i.ibb.co/FgwLrbT/Caesar-cipher.png)

The action of a Caesar cipher is to replace each plaintext letter with a different one a fixed number of places down the alphabet. The cipher illustrated here uses a left shift of three, so that (for example) each occurrence of E in the plaintext becomes B in the ciphertext.

| A | B | C | D | E | F | G | H | I | J | K | L | M | N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 | 25 |

When encrypting, a person looks up each letter of the message in the "plain" line and writes down the corresponding letter in the "cipher" line.

**Plaintext:**    THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG

**Ciphertext:** QEB NRFZH YOLTK CLU GRJMP LSBO QEB IXWV ALD

Deciphering is done in reverse, with a right shift of 3.

The encryption can also be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A → 0, B → 1, ..., Z → 25.[2] Encryption of a letter x by a shift n can be described mathematically as,

![caesarcipher_encode](https://i.ibb.co/MsxQqf2/function-encode.png)

Decryption is performed similarly,

![caesarcipher_decode](https://i.ibb.co/s3XDzdv/function-decode.png)

(There are different definitions for the modulo operation. In the above, the result is in the range 0 to 25; i.e., if x + n or x − n are not in the range 0 to 25, we have to subtract or add 26.)

The replacement remains the same throughout the message, so the cipher is classed as a type of monoalphabetic substitution, as opposed to polyalphabetic substitution.

# How to use program?

After the clone repository to your computer, run the **main.py** with Python3.

![caesar_cipher](https://i.ibb.co/ncC0ZMb/caesar-main.png)

Type which transaction you want, **encode** or **decode**.

After follow the instructions below. You will achieve encrypted/decrpyted text. 

# Encode

Type your text which you want to encrypt and specify your shift number.

![caesar_cipher](https://i.ibb.co/DWrK8pQ/caesar-encode.png)

# Decode

Type your **encrypted** text and write how many times shifted?

![caesar_cipher](https://i.ibb.co/ZmshkVh/caesar-decode.png)

If you are done with program type **"no'** to exit.

![caesar_cipher](https://i.ibb.co/ZVrCK4p/caesar-end-program.png)

# Weakness
If an attacker knows that the message has been encrypted using Caesar Cipher, he can try all shifts (b values from 1 to 25) to decrypt the message. This is called the **bruteforce** method.

