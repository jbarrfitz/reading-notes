# Class 18

**Date Due:** May 16, 6:30 pm PDT

## Reading

- [_Encryption, Decryption & Hacking_](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)
- [Caesar Cypher_](https://en.wikipedia.org/wiki/Caesar_cipher)
- [_How to Scrape Websites without Getting Blocked_](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

## Video

- [_Cryptography Crash Course_](https://www.youtube.com/watch?v=jhXCTbFnK8o)

## Reading Questions

### What is the basic principle behind the Caesar Cipher, and how was it used historically?

The Caesar Cipher is a basic alphabet-shift cipher, in which each character in the message is shifted by a set number in the alphabet.
It was recorded to have been used by Julius Caesar to transmit military messages. Caesar's use of the cipher is said to have had a
shift of three.

### What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?

Symmetric encryption uses a single, shared key for both encryption and decryption, while assymetric encryption uses a public key
for encryption and a private key for decryption. Symmetric encryption is largely used for securing larger data transfers, while
asymmetric encryption is used for secure communications and digital signatures, such as SSL/TLS.

### How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography

There are a couple ways that computers generate random number. True Random Number Generation (TRNG) involves observing some phenomenon
outside the computer and using that as a basis for generating the random number. These are items that cannot be predicted by any known
method and are truly random, such as the exact time a user interacts with a computer or the observation of some other outside resource.
Pseudo-random number generators, on the other hand, are usually generated using an algorithm within the computer itself. If someone
wanting to decrypt the random number understands the method by which the pseudo-random number is generated, they can reverse-engineer
the process to determine the original state. Pseudo-random number generators are generally unusable for cryptological purposes for this
reason.

### What’s the difference between encryption and decryption? Explain with an analogy

Encryption is the process of taking a plain text message and scrambling it in such a way that renders it unreadable to anyone who attempts
to intercept that message. Decryption is the opposite process, taking the scrambled message and applying a key to it to reassemble it
into a plain text, readable message. The process ensure that only someone who possesses the decription key will be able to read the
message. Encryption is akin to locking up valuable items in a lockbox with a combination, denying access to it to anyone who does not
have the combination to the lock. Possessing the combination allows you to access those items, which is similar to "decrypting" the lockbox.