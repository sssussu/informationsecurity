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


a) Install Hashcat. Test it with a sample hash. See Karvinen 2022: Cracking Passwords with Hashcat 

Install the apps
But fist update



- <img width="536" alt="Screenshot 2024-09-29 at 7 09 31" src="https://github.com/user-attachments/assets/b7464127-2a8e-48b1-b838-f3bf65745a00">

- <img width="537" alt="Screenshot 2024-09-29 at 7 09 59" src="https://github.com/user-attachments/assets/e200a718-01a9-4f8e-82a8-8d84b0d64d8c">


Create a new directory for our work

- <img width="398" alt="Screenshot 2024-09-29 at 7 32 21" src="https://github.com/user-attachments/assets/384ce401-c978-4a22-91fc-4ac089c125c4">

Get a big dictionary

- <img width="538" alt="Screenshot 2024-09-29 at 7 27 33" src="https://github.com/user-attachments/assets/8530a975-5447-445c-9fbc-07318be48ecc">


- <img width="380" alt="Screenshot 2024-09-29 at 7 29 27" src="https://github.com/user-attachments/assets/57703b7c-c64b-457f-bac2-bbd74759451b">

- <img width="112" alt="Screenshot 2024-09-29 at 7 29 47" src="https://github.com/user-attachments/assets/d466c8ef-720d-44fc-be87-ddccf7557406">

- <img width="513" alt="Screenshot 2024-09-29 at 7 36 37" src="https://github.com/user-attachments/assets/32caacc6-ec71-4a20-a113-86745246711c">


## Crack the Hash

- $ hashcat -m 0 '6b1628b016dff46e6fa35684be6acc96' rockyou.txt -o solved
- Installed: hashcat
- -m 0: type of the hash, identified using 'hashid' or 'hashcat' --example-hashes'
- '6b1628b016dff46e6fa35684be6acc96': The hash we want to crack
- -o solevd: save the solution as plain text to a new file "solved" in working directory

- <img width="521" alt="Screenshot 2024-09-29 at 7 46 55" src="https://github.com/user-attachments/assets/62055eea-c7a0-42cd-ac7a-b2cbed1816f2">


- <img width="422" alt="Screenshot 2024-09-29 at 7 47 33" src="https://github.com/user-attachments/assets/dcd7e9a3-b1f8-47b3-baf8-c1178ee32a94">

# b) Crack this hash: d595b2086532422bbe654bc07ea030df

- <img width="511" alt="Screenshot 2024-09-29 at 7 50 58" src="https://github.com/user-attachments/assets/39988aa5-905f-431d-a909-a3650c1d5cf2">


- <img width="524" alt="Screenshot 2024-09-29 at 7 56 19" src="https://github.com/user-attachments/assets/24e9a7d5-6d6d-491d-b155-19e1b8ade5c2">

- <img width="242" alt="Screenshot 2024-09-29 at 7 57 19" src="https://github.com/user-attachments/assets/6fc3ba08-b44b-4c60-8bd2-d7abb2e7a7c1">

## References
- https://terokarvinen.com/information-security/
- https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003
- https://terokarvinen.com/2022/cracking-passwords-with-hashcat/







