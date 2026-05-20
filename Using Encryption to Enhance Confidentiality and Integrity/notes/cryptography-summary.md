# Cryptography Summary

## Confidentiality

Confidentiality means preventing unauthorized people from reading data.

### Lab example

A plaintext message was encrypted into ciphertext. The ciphertext was unreadable until it was decrypted using the correct key.

---

## Integrity

Integrity means proving that data was not changed.

### Lab example

A digital signature was verified after decryption. Successful verification showed that the message had not been modified.

---

## Authentication

Authentication means proving the identity of a user or sender.

### Lab example

The sender signed the message using a private key. The recipient used the sender’s public key to verify the signature.

---

## Nonrepudiation

Nonrepudiation means the sender cannot easily deny that they signed the message.

### Lab example

The digital signature was tied to the sender’s private key.

---

## Symmetric Cryptography

Symmetric cryptography uses the same secret key for encryption and decryption.

### Strengths

- Fast
- Efficient for large files
- Common in bulk data encryption

### Weaknesses

- Secure key sharing is difficult
- Anyone with the secret key can decrypt the data

### Lab example

OpenSSL AES-256-CBC was used to encrypt a message file.

---

## Asymmetric Cryptography

Asymmetric cryptography uses a public key and a private key.

### Public key

Can be shared with others.

### Private key

Must be kept secret.

### Lab example

Kleopatra/GPG was used to create public/private key pairs. A message was encrypted using the recipient’s public key and decrypted using the recipient’s private key.

---

## Digital Signatures

Digital signatures use hashing and asymmetric cryptography.

### What they provide

- Integrity
- Authentication
- Nonrepudiation

### Lab example

A message was signed by the sender and verified by the recipient.

---

## Hybrid Cryptography

Hybrid cryptography combines asymmetric and symmetric encryption.

### Why it is useful

- Symmetric encryption is fast for data
- Asymmetric encryption helps securely protect or exchange the symmetric key

### Lab example

A message was encrypted symmetrically, and the secret key was protected using asymmetric encryption.

---

## Key Fingerprints

A fingerprint is a hash of a public key.

### Why it matters

Fingerprints help verify that a public key belongs to the expected person and has not been replaced or altered.

---

## Key Management Best Practices

- Protect private keys with strong passphrases
- Back up keys securely
- Verify public key fingerprints
- Revoke compromised keys
- Avoid publishing private keys or passphrases
- Use trusted channels when exchanging public keys
