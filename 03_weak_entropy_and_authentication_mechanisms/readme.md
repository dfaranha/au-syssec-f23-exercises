# Exercises: Weak Entropy and Authentication Mechanisms

## Exercise 1: Authentication Mechanisms

We will classify authentication mechanisms described in a set of printed slides according to the taxonomy we saw on class, and rank from the least secure to the most secure. The class will be split in at most 8 groups, each with its own set of slides. There will be two activities in the exercise:

1. First, classify all different authentication solutions into the 4 types given. Use the diagram below as a reference example. Consider that a user is authenticating against some service provider, and the classification should be performed from the point of view of the service provider and what authentication factors must be managed by it.

<p align="center">
  <img src="https://user-images.githubusercontent.com/5369810/134070931-a702ac64-8d96-45e1-a1fb-bc8846e572b9.png" />
</p>

2. After all solutions are classified, organize each column from **least** secure (on bottom) to **most** secure (on top).

**Observation:** _There is no single correct solution, the point is exactly to discuss the trade-offs. Assume a realistic implementation (not horrible or perfect) working in realistic conditions._

### Sample Solution (most to least secure)

Ownership Factors
* Authenticator App (most people often have their phones, good as a second factor)
* One-time Password Device (more likely to be lost than a phone with authenticator app)
* Credit Card with NFC (more secure than magnetic stripe)
* Cryptographic Token
* Cryptographic challenge-response
* Password Book (could be copied)
* Microchip beneath the skin (cannot be stolen, but very invasive and new technology)
* Credit Card (Magnetic stripe) (easy to copy)
* Government-issued ID card (relatively easy to forge or steal)


Multiple Factors
* NemID (password and app/number card)
* Credit Card with PIN and fingerprint (ownership & inherent)
* Credit card with chip and PIN (ownership & knowledge)
* University Access Card (ownership & knowledge)

Inherent Factors
* Keystroke Rhythm
* Fingerprint Scanning
* Gait Recognition
* Palm Scanning
* Iris Scanning
* Voice Recognition
* Face Recognition (easy to fool current face recognition)
* DNA Sample (might be possible to take a DNA sample from another person)
* Handwritten Signature (relatively easy to forge)


Knowledge Factors
* Password Manager (Master Password)
* Username/Password (many people use the same password for many accounts)
* Personal Identification Number (PIN) (sometimes short and easy to guess)
* Passphrase (sometimes easy to guess)
* Security Question (information could be easy to find or guess)

## Exercise 2: Weak Entropy

I have a big problem: When preparing this exercise last Tuesday, I encrypted a
very important file.  Unfortunately, I forgot to save the key, and now I cannot
access the data anymore.  Can you help me decrypt it?

This is the command that I used:
```
$ python encrypt.py plain.txt ciphertext.bin
```
