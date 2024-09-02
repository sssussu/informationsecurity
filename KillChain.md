# Kill Chain
### Cyber Kill Chain Paper
#### Summery of the articale 
##### Intelligence-Driven Computer Network Defense Informed By Analysis of Adversary Campaigns and Intrusion Kill Chains

The article explains and approaches different methods to protect computer networks from cyberattacks by studying how the attackers work. 
Firstly we are going to break down the title of the article so we can have a better understanding of every word and the meaning of it. 
1) By Computer Network Defense means protecting computer networks from cyber attacks.
2) Informed by Analysis of Adversary Campaigns includes studying the different patters and strategies used by the attackers in their past attacks.
3) Intrusion Kill Chains means a model that describes the steps that the attacker will take to succesfully breach in a network.

##### Abstract

The articale touched down in this part about the limitations of traditional network defenses like antivirus and basic detection systems and how they alone are not enough defending mechanism agaisnt advanced cyber threats specifically Advanced Persistent Threats (APT's). 
Advanced Persistent Threats refers to highly skilled, well-funded and targeted cyberattacks who breaks in a network  and remain undetected for an extended period of time. They target important and sensitive data like  economic, proprietary, or national security data.
### Introduction
##### Traditional Defense Tools and Their Limitations

Why the old defenses dosen't work ?
Conventional tools like detection systems and antivirus software focuses mainly on finding and fixing vulnerabilities in a system. They focus on fixing the weak spots in the system and react only after an attack has already happened.
As attackers's techniques evolve, these old methods are becoming less effective against more advanced threats. APT's can easily get past basic defenses.


The new ways to fight APT's: 
- Know your Enemy: Learn how the attackers operate
- defenders need to use an intelligence-driven approach that includes understanding methods used by the attackers.
- Constantly gather infromation about what the attackers are doing (intelligence feedback loop) where information about attackers is continuously gathered, analyzed, and used to improve defenses.
- This helps the defenders to predict any future attacks and reduce their success rate

To defend agaisnt APT's there is a need for an Intelligence-Driven Approach
Benefits of This Approach: 
- organizations can better prioritize their security investmen.
- this approach directly targets the attackers themselves, reducing their chances of success.

###### How to stop them?
- Kill Chain Model : Think of an attack as a chain with different steps. If you know the steps, you can stop the attack early, before it gets too far.
- Patters: Look for patterns in the attacks. By connecting the dots, you can see when similar attacks are part of a bigger plan.

Kill Chain model is a framework that describes the steps an attacker takes from planning to implementing the attack. By mapping the steps the defender can disrupt the attack at multiple stages.

Kill Chain Model: 
- Think of an attack as a series of steps or link in a chain.
- To succeed the attacker needs to get through each step without being stopped.
- Try to find ideas to interrupt the chain at any point to stop the attacker.

What's going on?
  -	APT’s are sending sneaky targeted emails to trick people into downloading harmful software.
  -	This software helps them steal sensitive information.

   Examples of APT' Attacks:
-
- Hackers managed to sneak into NASA and other U.S government networks stealing important information about rocket designs and more without getting caught.
-	They went after military and government systems to gather valuable information.

   What APT's attackers use? 
   - APT’s  uses special tools and unkown tricks called zero-day exploits that these defenses can’t detect.
If a software application has a security flaw that allows unauthorized users to gain access to sensitive data, and an attacker uses this flaw to steal that data, the flaw has been exploited.

The steps:
- Attacker finds a flaw or weakness in a system that can be exploited.
- Attacker uses methods and techniques to take advantage of the flaw.
- Attacker exploids the flaw.

## Releated Work

There are different ways to understand and defend against attackers and one of these ways is using something called kill chain.

Different models use step-by-step guides to understand and counter attacks. These guides help identify weaknesses and improve defenses

- Military Kill Chain : The U.S Department of Defense uses a kill chain with steps like finding, fixing, tracking.
- IED Attacks: For dealig with improvised explosive devices 
- Terrorism: The U.S Army has seven-step model to understand and counter terrorist planning.

ABSAC Framework:
- Focuses on countermeasures that deal with attacks at different stages, from early detection to dealing with ongoing attacks.

 Insider Threats: 
 - 	Problmes and risks can be caused also by people who are already inside an organization like employees or contractors ( this can be intentionally or accidentally).

Modelas: 
- Duran’s and Willson’s models are special tools or methods that help the organizations figure out how to spot and deal with these insiders threats.


##  Intelligence-driven Computer Network Defense
- This approach focuses on understanding the attackers themselves : what they can do, what they want, how they operate and what their weaknesses are.

How does it work?
Continuous Process:
- It’s always ongoing.
- You keep looking for clues called indicators that can show new attacks.
- Clues helps you find more clues that creates a cycle of learning and improving defenses.

If the defender can break even one link the attack will fail.
This approach makes defenses strong Since APT’s keep trying again and again each failed  attempt gives defenders a chance to learn and improve and if defenders can stop attacks faster than the attackers can change their methods  it becomes much harder and more expensive for attackers to succeed.

## Indicators and the Indicator Life Cycle
Types of Indicators: 
- Atomic Indicators (IP addresses, where the attack comes from, email addresses...)
- Computed Indicators ( Hash values )
- Behavioral Indicators

Indicators are clues that help detect and understand cyber attacks. They come in different types—simple facts, calculated data, and complex behaviors. Proper tracking of indicators is crucial to avoid errors and misinterpretations.

## Intrusion Kill Chain
A step-by-step process that attackers follow to break into a computer network, stay inside, and reach their goals. 

Steps in the Intrusion Kill Chain: 
 1.	Reconnaissance: Attackers look for information about their target.
 2.	Weaponization: Here, attackers create a tool (like a virus or trojan) that will help them get into the target system.
 3.	Delivery: This is how the attackers send their weapon to the target (sending emails...).
 4.	Exploitation: Once the weapon gets to the target it starts exploiding a weakness in the system.
 5.	Installation: The attacker installs a backdoor (secret access) on the victim’s computer. 
 6.	Command and Control: a communication tool between the computer of the system and the attacker.
 7.	Actions on Objectives: Attacker getting their full control over the data (exploided).

In this step if a defender can block even one of these steps they can stop the attack for example blocking a harmful email. 

## Courses of Action

The kill chain is a series of steps hackers take to carry out an attack. Defenders can disrupt the attack by acting at any step in the chain. 
Here's how:
1.	Installation: When the attacker installs a toll like a backdoor and the defender can can stop this by using antivirus software or restricting the system's ability to install unknown programs.
   
3.	Command and Control: Attacker will install their communication tools and the defender can block this communication by using firewalls or other network controls.
   
5.	Actions on Objectives: This is when hackers achieve their goals the dfenders can detect suspicious actions by monitoring logs or setting up traps (honeypots) that lure hackers into revealing their actions.

   ## Intrusion Reconstruction
Intrusion Reconstruction  is about piecing together all the steps an attacker took during a cyber attack so defenders can learn from it and prevent future attacks.

1.	Looking for Patterns
2.	Finding Key Indicators
3.	Understanding Attackers
4.	Indetifying and Tracking Campaigns
5.	Adjusting Defenses
6.	Tracking and Improving


   ## Campaign Analysis

Campaign Analysis helps defenders see the big picture of cyber attacks by finding patterns and key indicators across multiple attacks. This approach helps them predict and prevent future attacks more effectively.

## Intrusion Attempt 1 :
1.	The Setup: Suspicious email found with PDF document. This email was sent to just five people, who had been targeted before.
2.	The Trick: The email attachment was actually harmful. It used a known security flaw in Adobe PDF software.
3.	How It Worked: The harmful PDF had hidden code that would exploit the flaw in Adobe PDF. When someone opened the PDF, this code would run and install a backdoor on the victim’s computer.

The backdoor installed itself and began sending data to the attacker’s server. This was quickly interrupted by the defenders. In this case the Actions on Objectives phase wasen't reached.

Things that were similar:

- email came from the same sender.
- PDF file in the email used the same techniques as the previous attack.

 ## Intrusion Attempt 2:

On March 4, 2009, there was another attempt by the same attacker to break into a network using a similar method to the one from the day before. 

What Was different: 

- The new email was about a different topic
- The email was sent to different people
- The PDF file had a different name
- The email came from a different IP address address

What Analysts did:

- Recognized patterns
- Blocked the attack
- Gathered information to detect similar attacks in the future

What did they found: 

- Both attacks targeted similar groups and used documents from the same websites
- The harmful software used was the same in both cases
- Both attacks used the same security flaw in Adobe PDF

# a)Bookworm

For this task I used the detailed instructions that are found in terokarvinen.com webpage.

Firstly before installing virtual machine I downloaded Download Debian ISO image. I used this link
live amd64 folder on cdimage.debian.org and chose the debian-live-12.7.0-amd64-xfce.iso

<img width="391" alt="Screenshot 2024-09-02 at 2 29 40" src="https://github.com/user-attachments/assets/3b98c4f2-18f9-44e5-830c-b6a292391f76">

I already had installed the virtual boc in my computer so I only created a new virtual machine by selecting from menus, select Machine and New.

  <img width="449" alt="Screenshot 2024-09-02 at 2 34 20" src="https://github.com/user-attachments/assets/6e02cc51-c950-4dec-9f9d-c2ac3d011b0c">

  I created new virtual machine by clicking New. Then I click "Expert Mode" to get all the options in to my screen. Here is what it looked liked:
  
<img width="448" alt="Screenshot 2024-09-02 at 2 37 27" src="https://github.com/user-attachments/assets/ea502747-c48d-406d-be57-4e321c85f970">

Then I filled all the questions:
1. Name: DebianSelmaElCom
2. Type: Linux
3. Version: Debian (64-bit)
4. Memory Size: 4000 MB
5. Hard disk: Create a virtual hard disk now - yes
6. Hard disk File Location and Size: 60 GB

   <img width="446" alt="Screenshot 2024-09-02 at 2 40 19" src="https://github.com/user-attachments/assets/c9638344-0e3c-4c84-b457-8c813c0571e8">

   <img width="447" alt="Screenshot 2024-09-02 at 2 41 28" src="https://github.com/user-attachments/assets/db10363c-91c2-43c8-a603-c88e61e84114">

   Then at the end i clicked finnish to create my virtual machine.

   In this picture I had installed my virtual machine:
   
<img width="447" alt="Screenshot 2024-09-02 at 2 42 56" src="https://github.com/user-attachments/assets/fa9f13d7-9f3c-4dec-ab64-2a47e2ea0a17">

Then I selected my virtual machine from the left side of the screen and selected
settings --> Storage tab --> Under "Controller: IDE --> Then I chose the CDROM "Empty" --> On the right I chose "Optical Drive:" --> Then I  click the tiny CDROM icon to open a menu.

<img width="451" alt="Screenshot 2024-09-02 at 2 49 08" src="https://github.com/user-attachments/assets/fed7ea2b-2f0a-466b-83ba-ce63e57a8873">

After this I chose the Virtual Optical Disk File and selected my ISO disk image (debian-live-12.7.0-amd64-xfce.iso).

<img width="448" alt="Screenshot 2024-09-02 at 2 52 38" src="https://github.com/user-attachments/assets/8e71719a-e3c8-4924-8f99-710788babfc7">

Then I started to boot.

After booting I chose in my Boot Menu Live System (amd64).

<img width="319" alt="Screenshot 2024-09-02 at 2 55 11" src="https://github.com/user-attachments/assets/84c8bb56-ca40-43bc-8184-6d9a71ffee93">

Then I wanted to test the web browser so I chose from the left corner "Applications."

<img width="448" alt="Screenshot 2024-09-02 at 2 57 42" src="https://github.com/user-attachments/assets/904d2625-7187-446c-abb5-8dd9a4b6d203">

On top left I chose "Applications" --> "Web Browser".
To tests the basic functionality of mouse, keyboard, network and display I searched for Terokarvinen in the search bar.

<img width="453" alt="Screenshot 2024-09-02 at 3 00 47" src="https://github.com/user-attachments/assets/0e183e95-8caa-4240-a260-77b2943abdf1">

Then I clicked the "Install Debian" on homepage.

 <img width="450" alt="Screenshot 2024-09-02 at 3 04 04" src="https://github.com/user-attachments/assets/29d8b4be-2800-4e5f-b885-504a2f0939cd">

 After I filled all the information above: Location and Keyboard
 
<img width="449" alt="Screenshot 2024-09-02 at 3 04 58" src="https://github.com/user-attachments/assets/5ae06c2b-8168-4f73-bc1b-e25665b47c1f">

<img width="443" alt="Screenshot 2024-09-02 at 3 05 13" src="https://github.com/user-attachments/assets/7804383f-67f5-4599-92c7-44ec741dcf6f">

Then in Partitions I clicked "Erase disk" and chose from the bottom "book loader location" : "Master Boost Record of VBOX HARDDISK"

<img width="453" alt="Screenshot 2024-09-02 at 3 07 32" src="https://github.com/user-attachments/assets/1d616184-18f1-49ab-ad67-4677f45e72bc">

Then in users I filled all my user and password informations:

<img width="447" alt="Screenshot 2024-09-02 at 3 08 34" src="https://github.com/user-attachments/assets/a14bbd60-0cf4-4eb2-b9a3-a2101469c925">

After this I installed:

<img width="450" alt="Screenshot 2024-09-02 at 3 09 11" src="https://github.com/user-attachments/assets/1ac9d827-4e52-4642-b77a-2c07de038b76">

When I installed it it gave me "all done". I then clicked "Restart now" and the I clicked "Done".

<img width="449" alt="Screenshot 2024-09-02 at 3 10 34" src="https://github.com/user-attachments/assets/5e8fb2b5-8225-450f-8a72-cafce792c957">

After rebooting (reset) I kept clicking ESC while the computer was booting. 
Then I landed on GRUB Bootloader menu.
I chose DEBIAN GNU/Linux the the boot started again.

After booting i log in with my username and password and tried browsing in the internet again to make sure everythinf is okey. 

<img width="447" alt="Screenshot 2024-09-02 at 3 15 54" src="https://github.com/user-attachments/assets/45a9363d-eaab-4592-bb27-8d7c2b3ca33d">

After i made sure everything is okey I Open the terminal: Applications: Terminal Emulator.
Then I typed this command on the terminal: $ sudo apt-get update
<img width="450" alt="Screenshot 2024-09-02 at 3 18 19" src="https://github.com/user-attachments/assets/6717b09c-3430-49f6-ba19-4f3696d44898">

This command upgrades everything. After the upgrade is done I log in again into my virtual machine and open the terminal on type also $ sudo apt-get -y dist-upgrade command.


<img width="449" alt="Screenshot 2024-09-02 at 3 20 18" src="https://github.com/user-attachments/assets/5b0d48cd-09a9-49e9-9698-de6a1e1d35e9">

This installed the latest versions of all software.

Finally I installed a firewall by this command : $ sudo apt-get -y install ufw
$ sudo ufw enable


<img width="447" alt="Screenshot 2024-09-02 at 3 22 31" src="https://github.com/user-attachments/assets/0d43a7dd-76c9-4439-a5b2-10ed495c7e18">


And I reboot it. On top-left "Applications" menu: Log out: Restart.

Now my desktop is ready.

References:
https://terokarvinen.com/2021/install-debian-on-virtualbox/
https://terokarvinen.com
https://terokarvinen.com/information-security/
https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf


  


