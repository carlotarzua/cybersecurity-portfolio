# OpenSSL and File Commands

This file summarizes the command-line operations practiced in the lab. Sensitive values are sanitized for portfolio use.

## Generate an RSA Private Key

```bash
openssl genrsa -aes256 -out instructor_private.key 8192
```

### Purpose

Generates an encrypted 8192-bit RSA private key.

### Notes

- `genrsa` generates an RSA private key.
- `-aes256` encrypts the private key with AES-256.
- `-out` specifies the output file.
- `8192` specifies the key size.

---

## Generate a Public Key from a Private Key

```bash
openssl rsa -in instructor_private.key -pubout -out instructor_public.key
```

### Purpose

Creates a public key from the corresponding private key.

### Notes

- The public key is mathematically related to the private key.
- The private key should never be shared.
- The public key can be shared with others.

---

## Copy a Public Key

```bash
cp instructor_public.key /tmp
cp /tmp/instructor_public.key ~/
```

### Purpose

Copies the public key to a shared location, then retrieves it from another user account.

---

## Create a Plaintext Message File

```bash
touch secretmessage.txt
echo "Your Name" > secretmessage.txt
echo "Encrypted Message for Instructor" >> secretmessage.txt
cat secretmessage.txt
```

### Purpose

Creates a plaintext file, writes content to it, appends another line, and displays the contents.

---

## Encrypt a File with AES-256-CBC

```bash
openssl enc -aes-256-cbc -pbkdf2 -salt -a -e   -in secretmessage.txt   -out secretmessage_ENCRYPTED.txt
```

### Purpose

Encrypts a plaintext file using symmetric encryption.

### Notes

- `enc` uses OpenSSL encryption functionality.
- `-aes-256-cbc` specifies AES with a 256-bit key in CBC mode.
- `-pbkdf2` strengthens password-based key derivation.
- `-salt` adds randomness to make attacks harder.
- `-a` outputs base64 text.
- `-e` means encrypt.
- `-in` specifies the input file.
- `-out` specifies the encrypted output file.

---

## View Ciphertext

```bash
cat secretmessage_ENCRYPTED.txt
```

### Purpose

Displays the encrypted output. The ciphertext should not be readable like the original plaintext.

---

## Remove Plaintext

```bash
rm secretmessage.txt
```

### Purpose

Deletes the original plaintext file after creating the encrypted version.

---

## List Files

```bash
ls
ls *.key
```

### Purpose

Lists files in the current directory or lists key files specifically.

---

## Portfolio Safety Notes

Do not publish:

- Real passwords
- Passphrases
- Private keys
- Raw decrypted secrets
- Reusable symmetric keys
- Screenshots showing sensitive key material
- Instructor-provided lab instructions or answer keys
