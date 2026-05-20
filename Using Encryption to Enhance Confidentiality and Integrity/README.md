# 🎯 Encryption for Confidentiality & Integrity Lab

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-0A66C2?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Encryption](https://img.shields.io/badge/Encryption-2E8B57?style=for-the-badge&logo=letsencrypt&logoColor=white)
![GPG](https://img.shields.io/badge/GPG-0093DD?style=for-the-badge&logo=gnuprivacyguard&logoColor=white)
![OpenSSL](https://img.shields.io/badge/OpenSSL-721412?style=for-the-badge&logo=openssl&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

A hands-on cybersecurity lab focused on **cryptography, public/private key pairs, file encryption, digital signatures, symmetric encryption, and hybrid cryptography**.

This lab demonstrates how encryption protects confidentiality, how digital signatures support integrity and nonrepudiation, and how tools like Kleopatra/GPG and OpenSSL are used to encrypt, decrypt, sign, verify, and transfer protected files.

---

## ✨ Features

- 🔑 **Asymmetric Key Pair Creation** — Generated public/private key pairs using Kleopatra and GPG
- 🧾 **Public Key Exchange** — Exported and imported public keys between users
- 🧬 **Fingerprint Verification** — Reviewed key fingerprints to validate key identity and integrity
- 🔐 **File Signing & Encryption** — Signed and encrypted a message using public-key cryptography
- 📄 **Ciphertext Inspection** — Compared readable plaintext with encrypted ciphertext
- 🔓 **Decryption & Signature Verification** — Decrypted a protected file and verified the digital signature
- ⚡ **Symmetric Encryption** — Used OpenSSL with AES-256-CBC to encrypt a file
- 🧩 **Hybrid Cryptography** — Combined symmetric encryption with asymmetric key protection
- ✍️ **Digital Signatures** — Created and verified a digitally signed message using GPG

---

## 🚀 Demo

> The lab shows how a sender can encrypt a message for a recipient, sign it for integrity and nonrepudiation, and allow only the intended recipient to decrypt it.

```text
Create Key Pairs
        │
        ▼
 Exchange Public Keys
        │
        ▼
 Sign Message with Sender Private Key
        │
        ▼
 Encrypt Message with Recipient Public Key
        │
        ▼
 Transfer Ciphertext
        │
        ▼
 Decrypt with Recipient Private Key
        │
        ▼
 Verify Signature & Read Plaintext
```

> Note: Before publishing screenshots, remove or blur names, email addresses, timestamps, platform watermarks, key fingerprints if you do not want them public, passphrases, passwords, and any raw private-key material.

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Certificate / Key Management** | Kleopatra |
| **Cryptography Suite** | GPG4Win / GPG |
| **Command-Line Crypto Toolkit** | OpenSSL |
| **Asymmetric Cryptography** | RSA public/private key pairs |
| **Symmetric Cryptography** | AES-256-CBC |
| **Hashing / Integrity** | Digital signature verification |
| **Operating Systems** | Windows Server, Ubuntu Linux |
| **Security Concepts** | Confidentiality, integrity, authentication, nonrepudiation, hybrid encryption |

---

## 🧠 How It Works

```text
Plaintext Message
        │
        ▼
  Digital Signature  ─────────── Sender signs using private key
        │
        ▼
  Public-Key Encryption  ─────── Message encrypted using recipient public key
        │
        ▼
  Ciphertext  ────────────────── Unreadable protected output
        │
        ▼
  Private-Key Decryption  ────── Recipient decrypts using private key
        │
        ▼
  Signature Verification  ────── Recipient validates sender identity and integrity
        │
        ▼
  Recovered Plaintext  ───────── Message is readable again
```

1. **Generated OpenPGP key pairs** for the sender and recipient using Kleopatra
2. **Reviewed key fingerprints** to identify and validate public keys
3. **Exported and imported public keys** so each user could trust the other user’s certificate
4. **Created a plaintext message** and signed/encrypted it for the recipient
5. **Inspected ciphertext** to observe how encrypted data differs from readable plaintext
6. **Decrypted and verified the message** as the recipient using the recipient’s private key
7. **Generated RSA keys with OpenSSL** in Linux
8. **Encrypted a message symmetrically** using AES-256-CBC
9. **Protected the symmetric key using asymmetric encryption** to demonstrate hybrid cryptography
10. **Created and verified digital signatures** to validate message integrity and sender authenticity

---

## 📂 Project Structure

```text
encryption-confidentiality-integrity-lab/
├── README.md
└── notes/
    ├── key-takeaways.md
    ├── openssl-commands.md
    └── cryptography-summary.md
```

---

## ⚙️ Lab Summary

### Objective

Use encryption tools to protect confidentiality and integrity by generating key pairs, exchanging public keys, encrypting/decrypting files, and signing/verifying messages.

### Main Activities

| Area | What Was Practiced |
|---|---|
| **Key Pair Creation** | Created public/private keys using Kleopatra and OpenSSL |
| **Public Key Exchange** | Exported and imported public keys between users |
| **Certificate Trust** | Certified imported public keys in Kleopatra |
| **Asymmetric Encryption** | Encrypted a message using the recipient’s public key |
| **Digital Signing** | Signed a message using the sender’s private key |
| **Decryption** | Decrypted ciphertext using the recipient’s private key |
| **Verification** | Verified that the digital signature was valid |
| **Symmetric Encryption** | Used OpenSSL AES-256-CBC encryption |
| **Hybrid Cryptography** | Encrypted data symmetrically and protected the secret key asymmetrically |
| **Challenge Work** | Generated GPG keys, signed a document, and verified the signature |

---

## 🧪 Commands & Tools Practiced

### OpenSSL RSA Key Generation

```bash
openssl genrsa -aes256 -out instructor_private.key 8192
```

Generated an encrypted RSA private key.

```bash
openssl rsa -in instructor_private.key -pubout -out instructor_public.key
```

Derived a public key from the private key.

### Symmetric File Encryption

```bash
openssl enc -aes-256-cbc -pbkdf2 -salt -a -e   -in secretmessage.txt   -out secretmessage_ENCRYPTED.txt
```

Encrypted a plaintext file using AES-256-CBC.

### File and Directory Commands

```bash
touch secretmessage.txt
echo "message text" > secretmessage.txt
echo "more text" >> secretmessage.txt
cat secretmessage.txt
ls
rm secretmessage.txt
cp source destination
```

Used to create, view, copy, list, and remove files during the encryption workflow.

> Public portfolio note: do not publish real passphrases, passwords, raw private keys, or reusable encryption secrets.

---

## 🔐 Security Concepts Demonstrated

- **Confidentiality** — Encryption keeps information unreadable to unauthorized users
- **Integrity** — Hashing and digital signatures help prove that data was not changed
- **Authentication** — Public/private key relationships help verify the identity of a sender
- **Nonrepudiation** — A digital signature helps prove that a specific private key signed a message
- **Symmetric Cryptography** — Same key is used to encrypt and decrypt data
- **Asymmetric Cryptography** — Public key encrypts or verifies; private key decrypts or signs
- **Hybrid Cryptography** — Combines fast symmetric encryption with secure asymmetric key exchange
- **Key Fingerprints** — Short identifiers used to verify public key identity and integrity
- **Certificate Trust** — Users must decide whether to trust imported public keys
- **Key Protection** — Private keys should be protected with strong passphrases and stored securely

---

## 📸 Suggested Screenshots to Include Later

From the submitted lab report, the strongest portfolio screenshots would be:

| Screenshot | Why It Is Useful |
|---|---|
| **Key fingerprint for your key pair** | Shows public/private key generation |
| **Alice’s public key in your certificate cache** | Shows public key exchange and trust setup |
| **Successful signing and encryption message** | Shows encryption and digital signing workflow |
| **Ciphertext output** | Shows plaintext transformed into unreadable encrypted data |
| **Decrypt/Verify Files window** | Shows successful decryption and signature verification |
| **Instructor key pair files** | Shows OpenSSL key generation in Linux |
| **Ciphertext in encrypted message file** | Shows symmetric encryption output |
| **Encrypted secret key file** | Shows hybrid cryptography workflow |
| **Decrypted message file** | Shows successful recovery of protected data |
| **Successful signature verification** | Shows digital signature validation |

---

## 🧩 Key Takeaways

- Encryption supports confidentiality by converting plaintext into ciphertext.
- Asymmetric cryptography uses a public key and private key pair.
- A message encrypted with a recipient’s public key can only be decrypted with the matching private key.
- Digital signatures support integrity, authentication, and nonrepudiation.
- Public key fingerprints help verify that the correct key is being used.
- Symmetric encryption is faster, but securely sharing the secret key is a challenge.
- Hybrid cryptography combines the speed of symmetric encryption with the secure key exchange benefits of asymmetric encryption.
- Private keys and passphrases must be protected carefully.
- OpenSSL and GPG/Kleopatra are practical tools for encryption, signing, decryption, and verification.

---

## 🌱 Future Improvements

- [ ] Add sanitized screenshots of the encryption and decryption workflow
- [ ] Add a diagram comparing symmetric, asymmetric, and hybrid cryptography
- [ ] Add a table explaining confidentiality, integrity, authentication, and nonrepudiation
- [ ] Add a GPG command-line version of the Kleopatra workflow
- [ ] Add a short reflection on key management best practices

---

## 👩‍💻 About Me

Built by **Carlota Arzúa** — a cybersecurity student and developer interested in cryptography, infrastructure security, network security, and applied defensive security.

- 💼 [LinkedIn](https://www.linkedin.com/in/carlota-a-53a75b206/)
- 🌐 [Portfolio]()
- 📧 carlotaarzua@gmail.com

---

## 📄 License

This repository is for educational and portfolio purposes.

Do not redistribute instructor-provided lab manuals, answer keys, screenshots with sensitive information, credentials, private keys, passphrases, or copyrighted course material without permission.
