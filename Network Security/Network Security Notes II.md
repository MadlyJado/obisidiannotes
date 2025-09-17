
## Ciphers

- Ciphers are the algorithms that we use to encrypt and decrypt data from cleartext to ciphertext

Algorithm Types: 

AES - Symmetric
RSA - Asymmetric

Can be different bit lengths (Key Lengths)

128-bit (2^128)
256-bit (2^256)

## Symmetric vs. Asymmetric

What is Symmetric?

	Symmetric encryption is where one key is used for encrypting and decrypting from cleartext to ciphertext.

What is a key?

	A key is another input that is put into the cipher to encrypt and decrypt the data.

What is Asymmetric encryption?

	Asymmetric encryption is encryption where one key encrypts, and another key related to the other key decrypts.

Why would we use Asymmetric instead of Symmetric when Symmetric encryption is easier on the CPU?

Asymmetric encryption makes it so you can take one key, and can put it on the internet (Public), and send it to someone you wish to engage in a secure communication with.

If a user wishes to send you data securely, they encrypt the data with your public key, and send it to you. Only *your* private key can be used to decrypt the message.

## Stream vs. Block

Stream

- Stream input is when an algorithm can only input/output one bit at a time for encryption/decryption.
- Block input/output is when an algorithm can send "blocks" of data at a time through the cipher to encrypt/decrypt the data.


### How can we send a symmetric key securely, to create a secure session?

TLS creates a three way handshake, on top of TCP. This is how it works:

The Sender, sends their publickey, and a portion of a symmetric key (Could be AES, or some other symmetric key algorithm),

 


