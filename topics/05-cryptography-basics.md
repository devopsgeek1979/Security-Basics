# 05. Cryptography Basics

## Key Concepts

- **Encryption:** Converts plaintext to ciphertext.
- **Decryption:** Converts ciphertext back to plaintext.
- **Hashing:** One-way transformation for integrity checks.
- **Digital Signature:** Confirms authenticity and integrity.

## Symmetric vs Asymmetric Encryption

- **Symmetric:** Same key for encrypt/decrypt (fast, key sharing challenge).
- **Asymmetric:** Public/private key pair (slower, easier key distribution).

## TLS/HTTPS (High-Level)

1. Client and server negotiate protocol/cipher.
2. Server presents certificate.
3. Client validates certificate chain.
4. Session keys established.
5. Encrypted communication starts.

## Password Storage

- Never store plaintext passwords.
- Use strong password hashing (bcrypt/Argon2/scrypt).
- Add unique salt per password.
- Optionally add server-side pepper.
