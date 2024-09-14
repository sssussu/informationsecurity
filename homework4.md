# h4 Webbed 


## Broken access control

- Broken access control is when users perform actions or access data they aren't authorized to.
- Broken access control is common in the applicatios.
- Incidence Rate: 94% of applications were found with some form of broken access control.

### Common Vulnerabilities:
- Users accessing data or actions beyond their permissions.
- Modifying URLs or API requests to bypass access controls.
- Insecure handling of direct object references.
- Missing controls for POST, PUT, DELETE actions in APIs.
- Exploiting cross-site request forgery (CSRF) and other attacks.
- Misconfigured CORS leading to unauthorized access.

### How to prevent?
- Only handle access control on the server-side, where attackers can't mess with it.
- Block access to everything by default, then only give access when needed.
- Make sure all areas of the app follow the same security rules.
- Protect sensitive files and directories from being accessed.
- Log and monitor any failed access attempts.
- Use short-term tokens for login sessions and end them when users log out.

### Example attacks:

- Scenario 1: An attacker changes the account number in a URL and gets into someone else’s account.
- Scenario 2: An attacker can access admin pages without being an admin or even logged in.

## Security misconfiguration

Security misconfiguration is a common issue in web applications, occurring when systems or software aren't properly set up or maintained. This can include things like leaving default settings, failing to update software, or revealing sensitive information through error messages. 

### Vulnerabilities

- Incomplete security setup or missing security features across different parts of the app.
- Unnecessary features or services enabled, increasing the attack surface.
- Default accounts and passwords still active.
- Revealing too much information in error messages (like stack traces).
- Outdated software or security features not properly configured.

### How to prevent?

- Implement a secure, repeatable setup process for all environments (development, testing, production).
- Disable or remove any features or components that aren't necessary.
- Regularly review and update security settings, and apply patches promptly.
- Use proper cloud permissions to avoid accidental exposure of sensitive data.
- Automate the process of checking configurations and security settings.

### Example Attacks:

- Scenario 1: Sample applications left on a production server are exploited by attackers because they contain known vulnerabilities.
  
- Scenario 2: Directory listing is enabled, allowing attackers to access sensitive files and reverse-engineer the code to find security flaws.
  
- Scenario 3: Detailed error messages reveal sensitive system information, making it easier for attackers to find weaknesses.
  
- Scenario 4: Cloud storage permissions are left open, allowing unauthorized users to access sensitive data.


## Vulnerable and outdated components

Vulnerable and outdated components are a serious security issue that occurs when software or parts of a system, like libraries and frameworks, are not updated or maintained properly. 

his can leave systems open to attacks, and it's often hard to track which components are at risk.

### Vulnerabilities:

When outdated or unsupported components are used in software, it can lead to major security risks.

- Not knowing which versions of software components you're using.
- Using outdated, unsupported, or vulnerable software.
- Failing to regularly check for and apply security updates.
- Not testing how updates will affect the rest of the system.
- Leaving component configurations insecure.

### How to prevent?

- Continuously monitor the versions of both client-side and server-side components.
- Use automated tools to check for vulnerabilities and subscribe to security alerts.
- Only use components from trusted sources and prefer signed packages.
- Monitor for components that are no longer maintained and patch them if possible.
- Make sure you have a plan in place to keep systems secure over the lifetime of the application.

### Example attacks:

- Scenario 1: A vulnerability in the Struts 2 framework allowed remote code execution, which was responsible for several major data breaches.
- 
Scenario 2: IoT devices, which are often difficult to update, are at high risk if they aren't patched. An example is the Heartbleed vulnerability that affected many devices.

## Injection

Injection attacks happen when an application allows untrusted data to be processed by a database or system without proper checks, leading to security vulnerabilities. This includes attacks like SQL injection, where attackers manipulate queries to gain unauthorized access to data or systems.

Injection attacks occur when untrusted data is allowed to alter commands sent to databases or systems, like SQL, NoSQL, and OS command injections.

### Vulnerabilities:

- User input not being validated, filtered, or sanitized.
- Dynamic queries that directly use untrusted data.
- Using hostile data in object-relational mapping (ORM) or command executions.
- Concatenating untrusted data directly into SQL or commands.

### How to prevent it?

- Implement server-side validation to ensure inputs are safe.
- For dynamic queries, escape special characters specific to the interpreter.
- Use SQL features like LIMIT to prevent mass data exposure in case of an injection.


### Example attacks:

- Scenario 1: An SQL query takes user input directly without filtering, allowing an attacker to modify the query and access all accounts.
- Scenario 2: Insecure use of a framework like Hibernate can allow attackers to manipulate queries and delay responses, exploiting the system.


## a) Goat. Install WebGoat 2023.4.

Technical problmes reported.

I followed the Instructions but faced the same techincal problem. I tried tho install the latest version of WebGoat v.2028.8 and after several failed attempts I tried to download the v2023.4 (like in the instructions).

Detailed report for this task to make sure I followed every step.

### Installation of Java and Firewall:

I used: 
sudo apt-get update
sudo apt-get install openjdk-17-jre


- <img width="489" alt="Screenshot 2024-09-15 at 0 18 08" src="https://github.com/user-attachments/assets/2f3c262b-2d4c-4327-8369-c6f458498958">




- <img width="455" alt="Screenshot 2024-09-15 at 0 19 16" src="https://github.com/user-attachments/assets/2198ada2-bbec-4c30-905c-e0a9b5b643da">



By following the instructions the next step is to install a firewall by the following commands:

- sudo apt-get install ufw
- sudo ufw enable




<img width="527" alt="Screenshot 2024-09-15 at 0 20 53" src="https://github.com/user-attachments/assets/f8240022-7b0c-4a46-be14-b4b792503a8c">


### Trying with the v2023.4 (Trying with v2023.8 gave me the exact same results):

I started by downloading the webgoat-2023.4.jar

- <img width="518" alt="Screenshot 2024-09-15 at 0 30 37" src="https://github.com/user-attachments/assets/33641f30-2a63-4140-80fc-cbff3dd0097b">

I tried to download it several times because it showed me following error.

- <img width="415" alt="Screenshot 2024-09-15 at 0 32 16" src="https://github.com/user-attachments/assets/a5d1d2d9-eaa9-4cde-a4fb-26f75a86e771">

- <img width="415" alt="Screenshot 2024-09-15 at 0 33 37" src="https://github.com/user-attachments/assets/10fd7e50-bd9c-4dc1-a7cf-0546e4f4e28d">

- <img width="454" alt="Screenshot 2024-09-15 at 0 34 38" src="https://github.com/user-attachments/assets/69f79469-4b68-4135-9288-8d200b2394b1">

I still tried to download WebGoat JAR by using the following command:

$ wget https://github.com/WebGoat/WebGoat/releases/download/v2023.4/webgoat-2023.4.jar

- <img width="494" alt="Screenshot 2024-09-15 at 0 38 34" src="https://github.com/user-attachments/assets/d19a88cd-094b-421c-aba6-82ee85514c05">

The command can not be found. I tried to start from again, but the results remains the same.

Run WebGoat in an alternative port:

I tried using the following command (even if the previous steps didn't work out):

$ java -Dfile.encoding=UTF-8 -Dwebgoat.port=8888 -Dwebwolf.port=9090 -jar webgoat-2023.4.jar

- <img width="517" alt="Screenshot 2024-09-15 at 0 43 49" src="https://github.com/user-attachments/assets/7f4fde1d-343d-444e-9f42-9be149492587">


## b) F12. Solve WebGoat 2023.4: General: Developer tools

I couldn't start this task because of the failed attempt to download WebGoat in the previous task.

## c) Not outdated. Update all operating system and all applications in your Linux.

Updated by using:
- sudo apt update
  
- <img width="476" alt="Screenshot 2024-09-15 at 0 52 44" src="https://github.com/user-attachments/assets/1121e662-5411-48c9-a604-73be63c0145d">


- sudo apt upgrade
  
- <img width="464" alt="Screenshot 2024-09-15 at 0 54 35" ![Uploading Screenshot 2024-09-15 at 0.59.52.png…]()
src="https://github.com/user-attachments/assets/d85bba2c-9a9e-48d0-bd6a-fb9fc3fd05bc">

## d) 

### Select basics

- <img width="206" alt="Screenshot 2024-09-15 at 1 00 09" src="https://github.com/user-attachments/assets/f85ce054-8d41-4cb5-ab7b-517c84085a35">

- <img width="186" alt="Screenshot 2024-09-15 at 1 00 26" src="https://github.com/user-attachments/assets/23235570-d86e-41a0-9613-db1b11d07ce4">

### Select from world

- <img width="460" alt="Screenshot 2024-09-15 at 1 01 37" src="https://github.com/user-attachments/assets/1b91ec79-d9fb-4840-bf07-d8f3371a2517">

- <img width="162" alt="Screenshot 2024-09-15 at 1 02 11" src="https://github.com/user-attachments/assets/a0992dde-0268-4ca8-813f-9cae3e91e34e">

## e) Johnny tables

References: 
https://terokarvinen.com/information-security/#h4-webbed
https://owasp.org/Top10/A01_2021-Broken_Access_Control/
https://owasp.org/Top10/A05_2021-Security_Misconfiguration/
https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/
https://owasp.org/Top10/A03_2021-Injection/
https://terokarvinen.com/2023/webgoat-2023-4-ethical-web-hacking/
