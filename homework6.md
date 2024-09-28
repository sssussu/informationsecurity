# H6 September2024!

## x) Read or watch and summarize (This subtask x does not require tests with a computer. Some bullets per article is enough for your summary, feel free to write more if you like)
€ Schneier 2015: Applied Cryptography: 2.3 One-Way Functions and 2.4 One-Way Hash Functions.

## Protocol Building Blocks

- Purpose: Protocols organize cryptographic steps to solve problems like privacy and authentication between parties.
- Key Elements: Protocols must be clear, succesive, and agreed upon by all participants.
- Cryptographic Protocols: Use cryptography to prevent cheating and eavesdropping between distrustful parties.
- Challenges: Designing secure protocols is harder than finding flaws.
- Everyday Use: Formal protocols ensure fairness in digital interactions, like informal ones in real life.
- Key Players: Alice (initiator), Bob (responder), Eve (eavesdropper), Mallory (attacker), Trent (arbitrator).

### Arbitrated Protocols:
- A neutral third party, like a lawyer or bank, oversees transactions to ensure both parties act fairly.
- Example: When Alice sells a car to Bob, a lawyer holds the title until the payment clears.
- In computer networks, arbitrators are harder to trust, costly, and can slow things down.

### Adjudicated Protocols:
- Used when a dispute arises, involving a judge or adjudicator only when needed.
- Example: Alice and Bob sign a contract, but a judge steps in only if there's a disagreement.
- These protocols focus on detecting cheating, which discourages dishonest behavior.

### Self-Enforcing Protocols:
- No need for third parties; stops if cheating is detected.
### Attacks on Protocols:
- Passive: Eavesdropping (e.g., Eve).
- Active: Modifying messages (e.g., Mallory).
### Symmetric Cryptography:
- Secure communication using shared keys; key secrecy is vital.
### One-Way Functions:
- Easy to compute, hard to reverse; foundational in cryptography.
### Hash Functions:
- Convert inputs to fixed outputs; secure and collision-resistant.
### Message Authentication Codes (MACs):
- Hash with a secret key for data verification.
### Public-Key Cryptography:
- Uses public key for encryption and private key for decryption; simplifies key management.

## Hybrid Cryprosystems 

- Overview: Public-key algorithms arose with DES discussions, leading to community debates.
- Key Differences:
Public-key algorithms encrypt keys and are slower than symmetric algorithms.
They are vulnerable to chosen-plaintext attacks.
- Hybrid Process:
Bob shares his public key.
Alice encrypts a session key with it and sends it to Bob.
Bob decrypts the session key for secure communication.
- Merkle's Puzzles: Secure communication using encrypted puzzles without key exchange.
- Digital Signatures: Provide authenticity through a trusted arbitrator (Trent).
- Challenges: Reliance on Trent can create bottlenecks and security risks.


## Digital Signatures Quick Overview
- Digital Signature Trees: Merkle's infinite signature scheme.
- Public-Key Signing: Alice signs; Bob verifies.
- Features: Authentic, unforgeable, non-reusable.
- Timestamping: Prevents misuse.
- Hash Functions: Efficient signing of document hashes.
- Multiple Signatures: Supports signatures from several parties.
- Nonrepudiation: Compromise claims can occur.
- Applications: Used in treaties and agreements.

