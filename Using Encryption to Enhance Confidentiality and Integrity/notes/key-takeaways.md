# Key Takeaways

## Overview

This lab focused on using encryption to protect confidentiality and integrity. It used Kleopatra/GPG for public-key encryption and digital signatures, and OpenSSL for symmetric and hybrid cryptography workflows.

## Main Takeaways

### 1. Encryption protects confidentiality

Encryption transforms readable plaintext into unreadable ciphertext. Only someone with the correct key can decrypt the ciphertext back into plaintext.

### 2. Symmetric and asymmetric encryption solve different problems

Symmetric encryption is fast and uses the same secret key for encryption and decryption. Asymmetric encryption uses a public/private key pair and is useful when people need to communicate securely without first sharing a secret key.

### 3. Public keys can be shared, but private keys must be protected

A public key can be distributed to other users. A private key must remain secret and should be protected with a strong passphrase.

### 4. Key fingerprints help verify identity

A fingerprint is a hash-based identifier for a public key. It helps users confirm that they are using the correct public key.

### 5. Digital signatures support integrity and nonrepudiation

A digital signature helps prove that a message came from the holder of a private key and that the message was not changed after signing.

### 6. Signing and encryption can be used together

In the lab, the message was signed to prove sender authenticity and integrity, then encrypted to protect confidentiality.

### 7. Hybrid cryptography is practical for real systems

Hybrid cryptography uses asymmetric encryption to protect or exchange a symmetric key, then uses the symmetric key for faster data encryption.

### 8. OpenSSL is useful for command-line cryptography

OpenSSL can generate RSA keys, encrypt files with AES, and support hybrid encryption workflows.

### 9. Never publish secrets

Private keys, passphrases, passwords, decrypted secrets, and raw lab credentials should not be uploaded to a public GitHub repository.

## Reflection

This lab showed how cryptography supports the CIA triad, especially confidentiality and integrity. It also showed that encryption is not only about algorithms; key management, trust, fingerprints, passphrases, and verification are just as important.
