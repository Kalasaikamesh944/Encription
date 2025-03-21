# Encription
Encryption is a method of converting data into a code to prevent unauthorized access. There are many types of encryption algorithms, each with its own mechanism. Below is a list of some common encryption methods and their mechanisms:

---

### **1. Symmetric Encryption**
Symmetric encryption uses the same key for both encryption and decryption. It is fast and efficient for large amounts of data.

#### **Common Algorithms:**
- **AES (Advanced Encryption Standard):**
  - Mechanism: Uses a block cipher with key sizes of 128, 192, or 256 bits. It operates on 128-bit blocks and applies multiple rounds of substitution, permutation, and mixing.
  - Use Cases: Secure communications, file encryption, and VPNs.

- **DES (Data Encryption Standard):**
  - Mechanism: Uses a 56-bit key and operates on 64-bit blocks. It applies 16 rounds of substitution and permutation.
  - Use Cases: Legacy systems (now considered insecure due to short key length).

- **3DES (Triple DES):**
  - Mechanism: Applies DES three times with two or three different keys to increase security.
  - Use Cases: Legacy systems, but being phased out.

- **Blowfish:**
  - Mechanism: Uses a variable key length (32 to 448 bits) and operates on 64-bit blocks. It applies a Feistel network structure.
  - Use Cases: File encryption and secure communications.

- **Twofish:**
  - Mechanism: An improvement over Blowfish, it uses a block size of 128 bits and key sizes up to 256 bits.
  - Use Cases: Disk encryption and secure communications.

---

### **2. Asymmetric Encryption**
Asymmetric encryption uses a pair of keys: a public key for encryption and a private key for decryption. It is slower than symmetric encryption but more secure for key exchange.

#### **Common Algorithms:**
- **RSA (Rivest-Shamir-Adleman):**
  - Mechanism: Based on the difficulty of factoring large prime numbers. It uses modular arithmetic and generates public and private keys.
  - Use Cases: SSL/TLS, digital signatures, and secure key exchange.

- **ECC (Elliptic Curve Cryptography):**
  - Mechanism: Uses elliptic curves over finite fields to provide security with smaller key sizes compared to RSA.
  - Use Cases: Mobile devices, IoT, and SSL/TLS.

- **Diffie-Hellman:**
  - Mechanism: A key exchange algorithm that allows two parties to securely share a secret key over an insecure channel.
  - Use Cases: Secure key exchange in protocols like SSL/TLS.

---

### **3. Hash Functions**
Hash functions are one-way encryption methods that generate a fixed-size output (hash) from input data. They are used for data integrity and password storage.

#### **Common Algorithms:**
- **SHA (Secure Hash Algorithm):**
  - Mechanism: Produces a fixed-size hash (e.g., 256-bit for SHA-256) using a series of logical operations.
  - Use Cases: Data integrity, digital signatures, and password hashing.

- **MD5 (Message Digest Algorithm 5):**
  - Mechanism: Produces a 128-bit hash. It is now considered insecure due to vulnerabilities.
  - Use Cases: Legacy systems (not recommended for security).

- **bcrypt:**
  - Mechanism: A password-hashing function based on the Blowfish cipher. It incorporates a salt to prevent rainbow table attacks.
  - Use Cases: Password storage.

- **Argon2:**
  - Mechanism: A modern password-hashing function designed to resist GPU and side-channel attacks.
  - Use Cases: Password storage.

---

### **4. Stream Ciphers**
Stream ciphers encrypt data one bit or byte at a time, typically using a pseudorandom keystream.

#### **Common Algorithms:**
- **RC4 (Rivest Cipher 4):**
  - Mechanism: Generates a pseudorandom stream of bits (keystream) that is XORed with the plaintext.
  - Use Cases: Legacy systems (now considered insecure).

- **Salsa20/ChaCha20:**
  - Mechanism: Generates a keystream using a 256-bit key and a nonce. ChaCha20 is an improved version of Salsa20.
  - Use Cases: Secure communications (e.g., TLS).

---

### **5. Block Ciphers**
Block ciphers encrypt data in fixed-size blocks (e.g., 64 or 128 bits).

#### **Common Algorithms:**
- **AES (Advanced Encryption Standard):**
  - Mechanism: Encrypts data in 128-bit blocks using a symmetric key.
  - Use Cases: Widely used for secure communications and data encryption.

- **DES (Data Encryption Standard):**
  - Mechanism: Encrypts data in 64-bit blocks using a 56-bit key.
  - Use Cases: Legacy systems (now considered insecure).

---

### **6. Post-Quantum Cryptography**
These algorithms are designed to resist attacks from quantum computers.

#### **Common Algorithms:**
- **Lattice-based Cryptography:**
  - Mechanism: Uses mathematical problems related to lattices (e.g., Learning With Errors).
  - Use Cases: Future-proof encryption.

- **Hash-based Cryptography:**
  - Mechanism: Uses hash functions to create digital signatures.
  - Use Cases: Quantum-resistant signatures.

- **Code-based Cryptography:**
  - Mechanism: Uses error-correcting codes to create encryption schemes.
  - Use Cases: Quantum-resistant encryption.

---

### **7. Hybrid Encryption**
Combines symmetric and asymmetric encryption for efficiency and security.

#### **Mechanism:**
- Asymmetric encryption is used to securely exchange a symmetric key.
- Symmetric encryption is used to encrypt the actual data.

#### **Use Cases:**
- SSL/TLS, PGP (Pretty Good Privacy), and S/MIME.

---

### **8. Steganography**
Not strictly encryption, but a method of hiding data within other data (e.g., images or audio).

#### **Mechanism:**
- Embeds secret data within a carrier file without altering its appearance.

#### **Use Cases:**
- Covert communication.

---

### **9. Homomorphic Encryption**
Allows computations to be performed on encrypted data without decrypting it.

#### **Mechanism:**
- Uses complex mathematical structures to enable operations on ciphertext.

#### **Use Cases:**
- Secure cloud computing and privacy-preserving data analysis.

---

### **10. Lightweight Cryptography**
Designed for devices with limited resources (e.g., IoT devices).

#### **Common Algorithms:**
- **PRESENT:**
  - Mechanism: A block cipher designed for low-power devices.
  - Use Cases: IoT and embedded systems.

- **SPECK:**
  - Mechanism: A lightweight block cipher optimized for software and hardware.
  - Use Cases: IoT and mobile devices.

---

### **Summary Table**

| **Type**               | **Algorithm**       | **Key Size**       | **Mechanism**                              | **Use Cases**                     |
|-------------------------|---------------------|--------------------|--------------------------------------------|-----------------------------------|
| Symmetric               | AES                 | 128, 192, 256 bits | Block cipher with multiple rounds          | Secure communications, file encryption |
| Symmetric               | DES                 | 56 bits            | Block cipher with 16 rounds                | Legacy systems                   |
| Symmetric               | 3DES                | 112 or 168 bits    | Triple application of DES                 | Legacy systems                   |
| Symmetric               | Blowfish            | 32 to 448 bits     | Feistel network structure                 | File encryption                  |
| Asymmetric              | RSA                 | 1024 to 4096 bits  | Factoring large primes                     | SSL/TLS, digital signatures      |
| Asymmetric              | ECC                 | 160 to 521 bits    | Elliptic curve mathematics                | Mobile devices, IoT              |
| Hash                    | SHA-256             | 256 bits           | Logical operations on input data           | Data integrity, password hashing |
| Stream Cipher           | ChaCha20            | 256 bits           | Pseudorandom keystream                    | Secure communications            |
| Post-Quantum            | Lattice-based       | Varies             | Mathematical problems on lattices          | Future-proof encryption          |
| Hybrid                  | SSL/TLS             | Varies             | Combines symmetric and asymmetric methods | Secure web browsing              |

---

This list covers the most widely used encryption methods and their mechanisms.
