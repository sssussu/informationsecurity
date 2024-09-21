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

