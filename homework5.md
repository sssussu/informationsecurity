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

## a) Pretty Good indeed. Encrypt and decrypt a message with 'gnupg', using PGP public key cryptography. (Note that here you learn each step; for end users, you can often automate and make it look simple)

In this task we used gnuog tool to encrypt and decrypt messages using Pretty Good Privacy (PGP) public cryptoghraphy.

First we installed gnupg in the terminal by using following commands:

- sudo apt update
- sudo apt-get install gnupg


- <img width="539" alt="Screenshot 2024-09-22 at 1 59 12" src="https://github.com/user-attachments/assets/4a634dfc-7413-4a5d-a532-e46dbcc7e3cc">


- <img width="527" alt="Screenshot 2024-09-22 at 1 59 31" src="https://github.com/user-attachments/assets/92a3e323-a3ce-4682-9e3c-ad5028e5c9c3">






After Installing gnupg we generated Key pair: (Consist of a public and a private key)

- <img width="518" alt="Screenshot 2024-09-22 at 1 59 58" src="https://github.com/user-attachments/assets/9024474b-cbc2-4478-b513-b7f3533948ee">



We chose the option number 1 (RSA and RSA).
We chose a key size of 4096 bits.


- <img width="404" alt="Screenshot 2024-09-22 at 2 00 35" src="https://github.com/user-attachments/assets/53eb72a5-358c-4eac-8b2a-30996d34929e">



We chose the key to never expire.


- <img width="348" alt="Screenshot 2024-09-22 at 2 00 55" src="https://github.com/user-attachments/assets/2bb0c679-9011-419a-a444-70f597dcac4e">




We entered the name and email address.

- <img width="316" alt="Screenshot 2024-09-22 at 2 01 22" src="https://github.com/user-attachments/assets/9588ef50-2e00-40b3-9f6d-0dccfa25668b">


We created a passphrase to protect our private key and GPG will create key the key pair for it.



After this process we exported our public key by using the following command.

- gpg --armor --export selma.el@hotmail.fi > selma.key.asc


- <img width="542" alt="Screenshot 2024-09-22 at 2 02 01" src="https://github.com/user-attachments/assets/df642e37-327c-4203-9699-0070e82d7c0a">



After this proces the file have been exported in our directory.

Then we can share it with the person we want.

### Encrypt a message:
For this task we will need the other persons public key to encrypt a message.

In our case we already have the recipient's public key file. 

We imported the recipient public key by the following command:

gpg --armor --export selma.el@hotmail.fi > selma.key.asc


To import the recipient public key we wrote the following command:

- gpg --import recipient-public-key-asc.


Then we created a file name called mess.text by the following command:
- echo "This message is for you, keep it a secret" >mess.txt

- <img width="546" alt="Screenshot 2024-09-22 at 2 04 13" src="https://github.com/user-attachments/assets/9ce0631c-b31c-483e-8d94-935526878add">


To decrypt the message the recipient need to run the following command in the terminal:

gpg --decrypt mess.txt.gpg 


The recipient will get asked to enter our passphrase that we created before --> after this the message will be visible for the recipient.


## b) Password manager is open and cloudless. Choose a password manager that 1) works without the cloud and 2) is free, open-source software. Install it. Demonstrate its use. Explain why a password manager is needed i.e. what kind of attacks or threats it protects against.

### KeePassXC

For this task i chose the KeePassXC for a local, cloudless option. 

I started with installing KeePassXC by  the following command:

sudo apt-get installed keepassxc


- <img width="489" alt="Screenshot 2024-09-22 at 2 05 09" src="https://github.com/user-attachments/assets/7899995a-a189-45c3-867e-0c0f4fcd062e">

Then I typed in the command: keepassxc, an it opened like this:

- <img width="537" alt="Screenshot 2024-09-22 at 2 05 41" src="https://github.com/user-attachments/assets/2110ccb7-62b4-4e42-8271-5c62facd20a2">


Then I choose:
- Create a new database.
- select a strong master password.
- save the database file to a secure location in your computer.

Then i added an entry by selecting in the KeePassXC "Entries" menu --> New entry.



- <img width="547" alt="Screenshot 2024-09-22 at 2 06 39" src="https://github.com/user-attachments/assets/79dc4f69-2548-4de2-b6ca-51caf627fb22">


Then I added the following informations and repeated this process to add more accounts to my database.


- <img width="549" alt="Screenshot 2024-09-22 at 2 07 15" src="https://github.com/user-attachments/assets/773773e7-047c-4567-9c81-4663eaf2e2f8">



### Demonstrate its use

I opened the KeePassXC and unlocked the database by using the master password.


- <img width="544" alt="Screenshot 2024-09-22 at 2 07 41" src="https://github.com/user-attachments/assets/da244519-11f9-424c-9bac-98ccf2bf5636">



Then I had the acces to my entries again:


- <img width="536" alt="Screenshot 2024-09-22 at 2 07 57" src="https://github.com/user-attachments/assets/f92322ec-8f76-4848-9614-e72c8114f1f3">


Now I have acces to my passwords!

### Why password manager is needed

Using password manager is protecting you against:

- Phishing Attacks: password managers help you fill in passwords only for legitimate sites, reducing the risk of falling for phishing scams.
- Password Reuse: they allow you to generate and store unique passwords for each service, protecting against breaches on one platform affecting others.
- Weak Passwords: password managers can generate strong, complex passwords, enhancing your security.
- Memory Overload: they securely store passwords, so you don’t have to remember them all.


Conclusion
A password manager helps secure your digital life against various threats by ensuring that your passwords are strong, unique, and stored securely. This reduces the risk of unauthorized access to your accounts.

References:

https://terokarvinen.com/2023/pgp-encrypt-sign-verify/
https://terokarvinen.com/information-security/
https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec006


















