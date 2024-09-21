# h5 Urryb, Greb
## Read and summarize: Applied Cryptography: Chapter 1: Foundations

### Sender and Receiver
- A sender sends a message securely to a receiver.
- The goal is to prevent eavesdropping.

### Messages and Encryption
- A message in its original form is called plaintext or cleartext. --> Plaintext (M) is the original message.
####  Encryption: The process of disguising the message, turning it into ciphertext (C).
####  Decryption: Reverses the encryption, recovering the plaintext.

### Terminology
- Cryptography: Practice of securing messages.
- Cryptanalysis: Practice of breaking encrypted messages.
- Cryptology: The field including boths cryotography and cryptoanalysis, practiced by cryptologists.

### Encryption and Decryption Functions:
- Encryption function: E(M) = C
- Decryption function: D(C) = M
- Encryption followed by decryption returns the original message: D(E(M)= M

### Cryptographic Goals
- Authentication: Veryfying the sender's indentity.
- Integirty: Ensuring the message wasn't changed during transmission.
- Nonrepuditation: Preventing the sender from denying that they sent the message.

### Algorithms and Keys:
- A cryptographic algorithm (or cipher) handles encryption and decryption.
- Restricted Algorithms: Methods that depend on keeping the algorithm secret are now considered outdated and insecure.
- Modern systems use a key (K) to encrypt and decrypt messages.
- Encryption and decryption functions depend on the key: EK(M)=C, DK(C)=M.
- Some systems use different keys for encryption (K1) and decryption (K2): EK1(M)= C, DK2(C)=M.
- Security relies on the key, not the algorithm. If the key is secret, even if the algorithm is public the message remains secure.
- Cryptosystem: A combination of the algorithm all possible plaintext, ciphertexts and keys.

### Symmetric Algorithms
- Use the same key for encryption and decryption.
- Key must remain secret for security.
- Types:
  Stream algorithms: Encrypt bit by bit.
  Block algorithms: Encrypt fixed-size blocks.

### Public-Key Algorithms:
- Use a public key for encryption and a private key for decryption.
- Public key can be shared byt the private key must remain secret.

### Cryptanalysis
- Aim: Recover plaintext or keys without access.
- Assumes security relies on the key and not the algorithm.

### Attack types:
- Ciphertext-only: Analzyzes chiphertext to extract keys.
- Known-plaintext: Use known plaintext and ciphertext.
- Chosen-plaintext: Attacker selects plaintext for encryption.
- Adaptive-chosen: Modifies plaintext choises based on results.
- Chosen-ciphertext: Attacker selects chihertexts to decrypt.
- Chosen-key: Knowledge of key relationships.
- Rubber-hose: Coercive methods ot obtain keys.

### Attacks
- Known/ Chosen- Plaintext attacks: Common methods where cryptanalyst access encrypted messages or choose plaintexts for encryption.
- Historical use: Effective during WWII against enemy codes.

### Security Principles
- Kerckhoffs's Principle: Security relies on the key, not algorithm secrecy.
- Unconditional Security: Only the one-time pad is unbreakable.
- Computational Security: Algorithms should resist breaking with current or future resources.

### Attack Complexity
- Types: Data, processing, and storage complexities define the difficulty of attacks.

### Codes vs. Ciphers
- Codes: Use fixed phrases; less flexible.
- Ciphers: Encrypt any data type; more versatile.

### Steganography
- Hides secret messages within other messages ( example: using invisible ink or altering images).

### Chihers
- Substitution Ciphers: replace characters.
- Types: simple, homophonic, polygram, polyalphabetic.
- ROT13: simple rotation cipher.
  
Security:
- Simple ciphers are easy to break.
- Complex ciphers require more effort but can still be broken.

### Transposition Chipers
- Function: rearrange characters; vulnerable to frequency analysis.

### Rotor Machines
Function: mechanical encryption devices.

### One-Time Pads
- Definition: Perfect encryption with a random key used once.
- Method: Encrypts plaintext by adding key characters (mod 26).
- Security: unbreakable if keys are random and never reused.
- Key issues: requires key length = message length.
- Use: ideal for ultra-secure communications.

### Computer Algorithms
Common Types:
- DES: symmetric encryption standard.
- RSA: public-key for encryption/signatures.
- DSA: public-key for digital signatures only.

### Large Numbers
- Purpose: use physical analogs to illustrate large cryptographic numbers.

