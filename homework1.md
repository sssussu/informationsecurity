# Should Tero wear a helmet?
## Threat modeling manifesto
### What is threat modeling? 

Threat modeling is a process used in early stage of planning a system, project or any organization to protect their security from any potential concers and threats.

In threat modeling we analyze, manage and highlight any threats for the security system.

By indentifying threats in early stage we can create a more succesful system that is protected from hackeers or any other kind od security risk.

#### when we threat model, we ask four key questions:

1. What are we working on?
2. What can go wrong?
3. What are we going to do about it?
4. Did we do a good enough job?

This four key questions are vey essential in threat modeling. By answering all of this questions we can build a good security system for a company in example.

#### Why treat model?

- While performing threat modeling we can realise all the things that can go wrong in a system and potentially prevent from any future damages that could come at high price.
- It allows us to indentify design and implementation problems that needs to be fixed whether it is in a early stage or during the entire life of the system.
- The results we get from threat modeling can be used to improve the system.

#### Who should threat model?

Anyone with a individual or larger system who is concerned about the safety and the security of their system.

#### How should I use manidesto?

- You can use it as a guide to improve your own idealodgy about a therat model.
- By following the guidance in manifesto we can result in more effective and succesfull threat modeling.
- Use the ideas that manifesto provides for your own advantage.

#### The values that manifesto shares:
 1. A culture of finding and fixing design issues over checkbox compliance
 2. People and collaboration over processes, methodologies, and tools.
 3. A journey of understanding over security or privacy snapshot.
 4. Doing threat modeling over talking about it.
 5. Continuous refinement over a single delivery.

#### Principles of manifesto:
1. Threat modeling works best when you use it continously.
2. It should fit with how you and your team work and build and keep up with any design changes in small and manageable steps.
3. The results of threat modelignare useful when they matter to the people who are involved.
4. Talking openly helps everyone understand what needs to be done and writing things down keeps track of those agreements and lets you measure progress.

#### Patterns that benefit threat modeling
 - Systematic Approach: Be thoughfull and consistent by using security and privacy knowledge in an organized way.
 - Informed creativity: use practical skills combining scientific methods.
 - Varied Viewpoints: Bring together a diverse team with experts from different areas to work together.
 - Useful Toolkit: Use the right tools to make your work easier, more efficient, and measurable.
 - Theory into Practice: Apply previous proven techniques that fit your needs.

#### Patterns that inhibit threat modeling
- Hero Threat Modeler: One's individual skill is not enough to succesfully threat model.
- Admiration for the Problem: Don’t just focus on the problem; work on finding practical and useful solutions.
- Tendency to Overfocus: Don't focus in one area alone. Keep your eyes on the whole system as everything is depended on each other in threat modeling.
- Perfect Representation: There’s no one perfect way to show a threat model. Use different views and models to catch different issues.

  ### Adam Shostack videos explained with key points

  #### Why threat modeling?
  - We use threat model to anticipate problmes when it's still inexpensive to deal with them.
  - Ideally this means before any code has been written.
  -  We are thinking through what are we going to build and how are we going to arrange the components in case we need quick changes.
  -  Threat modeling is a set of methods that allows us to think about the security at that point, so that the thing we build is as secure as we need it to be.

 #### The four question framework for threat modeling

 - What are we working on?
 - What can go wrong?
 - What are we going to do about it?
 - Did we do a good job?

If you ask yourself those 4 questions you are already threat modeling.

#### Collaborating to answer: What are we working on?

- When we think about threat modeling we are thinking about whiteboards (sketching).
- The value of collaboration gives us the opportunity for different people to be drawing simultaneously.
- Collaborating helps us answer the question: "What are we working on?".

#### Sketching in threat modeling
- By sketching we are starting to answer what are we working on.
- We can sketch by using different tools like whiteboards.
- When we are sketching we are starting to put our ideas into a form that other people can engage with and can respond to.
- We sketch the improve the first thing that comes up to our head which is imperfect (we aknowledge our idea and start to improve it).

#### Record your threat modeling work
- The things we are building can require that we have records of them for future purposes (job...)
- Whiteboards can be insufficient.
- Therse is a business reason to develop a document of record.
- We can learn new details about the systems we are working on and feed all those details into the question of what can go wrong?

#### Data flow diagrams in threat modeling

Data flow diagrams are associated with threat modeling because threats tend to follow data.

Data flow diagrams are simple to draw and easy to use to help us understand what we are working on.

There are 5 symbols in data flow diagrams which are the following:

1. External entities: anything that is outside of your control.
2. Processes: Things that are under your control like running code that is yours.
3. Data flows: We use this element to connect external entities with processes.
4. Data store: Where we store our data.
5. Trust boundary: We show that different elements are operated by different entities and that we trust them differently.

With these elements we can make up a data flow diagrams.

#### What can go wrong?
- The heart of threat modeling is answering the question: What can go possibly worng?
- Asking ourselves that question is all we need to do express our concerns.
- When we don't know what we are looking for we can use for guidance STRIDE or a kill chian to help us answering the questions.

#### Introducing STRIDE for threat modeling
- Adding structure (in this example STRIDE) to how we answer the question what can go wrong.
- The reason we add a structure is to get a degree of consistency in the answers we produce.
-  mnemonic STRIDE  is one of the most important structures.
-  STRIDE stands for: Spoofing, Tampering, Repudication, Information disclousure, Denial of service and Elevation of privileges.
-  In each of the steps of STRIDE is a problem that occurs in systems from desktop software to cloud IoT to mobile.
-  With STRIDE we can improve our threat modeling and get better answers by thinking about each of these possible problems.

#### What are we goign to do about it
- We are going to track our work.
- We are going to aswer the question of the set of threats that we have discovered.
- Each need have to have something done about them. ( do somwthing about it)

#### What to do about it? Risk management
- There is a link between risk management and asnwering the question what are we going to do about it.
- Risk management is applied to a subset of the threats we discover in threat modeling to help us make a decision about what we're going to do about it.
- Threat modeling iforms us about risk management and that's how the link between risk management and asnwering the question what are we going to do about it comes together.

#### Did we do a good in threat modeling
- To answer this question we can ask ourselves: Would you recommend threat modeling to a colleague.
  

## a) Security Hygiene

Here are some basic security hygiene practices that everyone should follow, whether you are an idividual or a company.

- Use Strong Passwords
- Enable Two-Factor Authentication
- Keep Software Updated
- Use Antivirus and Anti-Malware Tools
- Backup Data Regularly
- Be Cautious with Emails and Links
- Use a Firewall
- Secure Your Wi-Fi Network
- Lock Your Devices
- Practice Safe Browsing
- Limit Data Sharing
- Educate Yourself and Others

## b) Make-belief boogie-man

For this task i chose for my imaginary company a taxi application for a company called QuickRide.

#### What are we working on?

A application where you can easily book a taxi for yourself.

Name of the company: QuickRide

Description: QuickRide is a taxi application that connects passengers with drivers through a mobile app. In the application you can book yourself a taxi, track your driver, get information about the driver, see the availability of the drivers, book ahead a ride and communicate with the driver.

It handles user data, payment transactions, and communication between passengers and drivers.

#### Assets

- Customer Data: Personal information of users(passengers and drivers), including names, phone numbers, email addresses, and payment details. This is a crown jewel.
- Payment Information: Credit card and payment details of users.
- Application Infrastructure: Servers, databases, and network infrastructure that support the app.
- Customer Support Systems: Tools used by the staff to assist users and resolve their issues.

#### Prioritization of Key Assets
- Customer Data: This is a high priority due to privacy implications.
- Payment Information: This is also a priority due to financial risk and regulatory.
- Driver Data: This is important but secondary to customer data and payment information.
- Infrastructure: This is essential for the operations of the mobile app but less sensitive than data.

#### Security Supports Business
- Customer Trus: With this we mean protecting customer and payment data builds trust between the customer and ensures continued business.
- Regulatory Compliance:  By ensuring data security we can meet legal requirements and avoid penalties.

#### System Diagram
- User Devices: This means smartphones with QuickRide app installed.
- Mobile App: Interface for booking rides, making payments, and communicating with drivers.
- Backend Servers: This includes data processing and transaction handling.
- Database: In database we strore customers data, payment information and drivers details.
- Payment Gateway: Makes sure and processes that financial transactions are made securely.
- Customer Support: Tools for handling issues that the customers faces.

#### Customer touchpoints
To ensure that we serve the customer rightfully we need:

- Booking Rides: Users interact with an mobile app to request and schedule rides.
- Payment Processing: Users enter payment information and make transactions
- Customer Support: Users have the chance to contact staff for support via mobile app.

#### What can go wrong?

STRIDE Model:
- Spoofing: Attackers might try to pretend to be someone else to the passenger or the driver.
- Tampering: Attackers could modify payment information
- Repudiation: Users or drivers might deny any transactions or actions.
- Information Disclosure: Sensitive data could be exposed if not properly protected.
- Denial of Service:  Attackers could disrupt the app’s availability or performance.
- Elevation of Privilege: Attackers can get unauthorized acces to user data or admin features.

#### Attack trees

- Exploiting a vulnerability in the payment gateway.
- Unauthorized access to customer payment information.

#### Some examples of identified risks:

- Data Breach of Payment Information: This have high risk due to financial impact and regulatory penalties.
- Insider Threats:  This have medium risk if employees misuse acces to sensitive data.

#### Prioritization of Risks

- Data Breach of Payment Information: This have the highest priority due to severe impact on financial and regulatory aspects.
- Insider Threats: This is notable but less immediate compared to external threats.

#### Targeted Threat Actors

- Cybercriminals: They often target financial data and personal information
- Hacktivists: Could for example target the company to make political statement.
- Insiders: Employees that have acces to sensitive information might cause a risk.

#### Known Tactics, Techniques and Procedures (TTPs)
- Phishing: This is used for stealing credentials.
- SQL Injection: This is used to exploied vulnerabilities in the app or database.
- DDoS Attacks: This is used to disrupt service availability.

#### Capability, Opportunity and Intent (COI)
- Capability: This means cybercriminals have the technical skills and tools.
- Opportunity: This means any vulnerabilities in the app provides entry points for the attackers.
- Intent: This includes financial gain, data theft, or disruption.

#### Business Continuity
To ensure we have succesfull business continuity we have  to have:
- Customer Trust
- Operational Continuity : We must keep the service (mobile app) running smoothly to meet user needs and regulatory requiremenets.

#### What are we going to do about it?

Here are some effective mitigation Strategies:
- Reduce Attack Surface: This means limiting exposure by minimizing access points and regularly updating the app.
- Limit Entry Points: With implementing strong authentication, secure coding practices, and network security measures.
- Mitigate: With using encryption for data transmission and storage and  regularly updating the  software.
- Eliminate: with removing any unnecessary feature that may cause vulnerabilities in the system.
- Transfer: By considering cyber insurance to cover potential financial losses.
- Accept: By accepting certain risks if mitigation is not achievable.

#### Did we do a good enough job?

We can evaluate our threat modeling by the following methods:

- Security Audits: By regularly performing detailed checks to evaluate security.
- Penetration Tests: By performing a test we can  identify what's wrong and fix vulnerabilities.
- Assessments: With continuous evaluate and improving security measures.
- Continuous Threat Modeling: By regularly updating the threat models based on the new threats and the chnages that can happen in the system.

#### Process: 

 Security is an ongoing process and not a one-time task. By regularly reviewing and updating the threat models we can esnure a continued protection.

 ## References:

 https://terokarvinen.com/information-security/
 https://www.threatmodelingmanifesto.org
 https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf
 https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
 https://darknetdiaries.com
 Chat gpt
 




   
