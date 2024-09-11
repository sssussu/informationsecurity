
# Hack to learn Hacking

## x) Summery of Disobey presenatation

### I Was Almoust a Cybercriminal - Sergey Ichtchenko (Youtube video)

#### Who is Sergey Ichtchenko
- 21 years old
- security consultat at WithSecure (2022-)
- Mathematics student at the University of Helsinki (2022-)
- Board member at Testausserveri ry (2023-)

#### What is testausserveri ry?
-An organisation that promotes coding and cyber security as a hobby amoung young people.
- Testausseveri ry have discords server, events, community open-source projects, competitions and societal work.
- They have 1700+ online members.
- 150+ organisastional members.

#### Cybercrime

Cybercrime rate during 2008-2022:
- Ages from 15-17: 76
- Ages from 18-20: 30
- Ages from 21-24: 14
- Ages from 25-29: 60
- Ages from 30-39: 47
- Ages from 40-49: 17
- Ages from 50-59: 6

#### Servey

Firsthand experience

- Anonymous servey of Testausserveri members.
- Thye got 36 responses.

The questions they asked in the servey were the following:

- How do the young people gain there interest ? (programming, hacking...)
- Answers: Family, curiosity and games.

- Who are these people?
- Stereotypes: People who don't go outside, lack of social skills, loners, no other hobbies.
- The Truth: They can look like anything and anyone!

- Why do some young people misbehave online or commit cybercrimes?
- Answers: Bad influence, for fun and for attention-seeking.

#### Sergyes Personal story

- Parents influenced him to start programming.
- He have been programming ever since he was little
- Knew what CTF's where.

#### Why did He get in to the cyber?
- out of curiosity and boredom.
- pocking around things he should not be pocking at.
- He saw "Linnanmäki" publishing on their website that anyone can get a 6 month pass if the pay 300 euros. They will get an activating code. Sergey figured out how to hack in a way that if you activate the wrong code you will get the 6 month pass. Instead of him actually hacking the website he decided to contact Linnanmäki for the following reasons:

- He new that reporting the issue that the application had was a good idea.
- He got rewarded.
- He got thanked.
- The issue got fixed.
- Hes parents where proud of him.


## Interventions

What to do if you want to raise a cybercriminal? 
- punish them.
- Give detention.
- Confiscate phone.
- Tell them to not do it again.
- Threaten them with legal action.




## a) Bandit oh-five. Solve Over The Wire: Bandit the first five levels (0-4)

#### For this Task i found it very hard to complete every level. I tried first with MacBook but unfortunately I did not take any screenshots of my process since it was a failed attempt. I would get "this command can't be found" after several tries attempts. After this I switch my PC from ios to windows. This was still not a full succes but a step closer to the final goal.

#### Level 0

First I started with installing the ssh server by the following command: 

sudo apt install openssh-server: 

<img width="529" alt="Screenshot 2024-09-11 at 23 29 08" src="https://github.com/user-attachments/assets/14a75760-143d-4f79-82ad-84f203a1ab0c">


After Installing the ssh server I opended it and logged in to bandit.




<img width="457" alt="Screenshot 2024-09-11 at 23 33 16" src="https://github.com/user-attachments/assets/41dcba3d-7b20-4124-acf9-4f39e64d89e9">




As you can see from the picture I failed to enter the game.
I tried again to get acces to the shh server by the following command: sudo systemctl status ssh.





<img width="483" alt="Screenshot 2024-09-11 at 23 35 51" src="https://github.com/user-attachments/assets/1f256418-77ef-42da-ab84-e114cdac3f1c">




After this I could get into the bandit by logging in.



<img width="400" alt="Screenshot 2024-09-11 at 23 36 26" src="https://github.com/user-attachments/assets/2cac78c4-2a95-4588-b1f2-40b26a8c2617">




<img width="329" alt="Screenshot 2024-09-11 at 23 37 53" src="https://github.com/user-attachments/assets/b3f5dc73-c981-4d49-b7f9-1436844da8b2">




I succeded to log into the bandit by using ssh server and connecting via bandit.labs.overthewire.org on port 2220

#### Level 0-1

The password for the this level is stored in the readme file. Here is how I got acces to the password.

<img width="407" alt="Screenshot 2024-09-11 at 23 43 49" src="https://github.com/user-attachments/assets/3a26e96c-3cb6-4c13-ba92-409ac61ba7c9">




<img width="393" alt="Screenshot 2024-09-11 at 23 44 14" src="https://github.com/user-attachments/assets/00ac4800-72e0-4e14-88d5-ec310d8fdf40">





<img width="391" alt="Screenshot 2024-09-11 at 23 44 47" src="https://github.com/user-attachments/assets/7fa491af-fa91-4bf1-8c3a-0dc17ce7bc55">

#### Level 1-2

In this level I faced many difficulties. I couldn't log in to the next level by using the bandit1 password from readme. I got very confused and tried multiple times to restart the game from the beggining. This is what I got out of it.

#### Level 2-3

<img width="305" alt="Screenshot 2024-09-11 at 23 48 30" src="https://github.com/user-attachments/assets/5bc4e1ab-7360-4c80-a13f-3d6daa65548c">





<img width="490" alt="Screenshot 2024-09-11 at 23 48 56" src="https://github.com/user-attachments/assets/8f678d10-2e2a-4120-a393-ebc5f5055f26">






<img width="522" alt="Screenshot 2024-09-11 at 23 49 31" src="https://github.com/user-attachments/assets/e8c76597-8397-4893-a4fc-59ea13863553">

## b)  Can't fish

#### In this following task I needed to disable networking and show that packets don't go trough. For example, by using 'ping 1.1.1.1' (Cloudfare DNS server) or 'ping 8.8.8.8' (Google DNS server).

For this task I used the ping command (ping 8.8.8.8) to connect to Google DNS. 
I disabled the internet connection from my virtual machine by going to --> settings --> network --> not attatched.

The I used the command ping 8.8.8.8 and got "network is unreachable#


<img width="284" alt="Screenshot 2024-09-11 at 23 56 31" src="https://github.com/user-attachments/assets/050a456d-5b43-4a49-a20d-907169a6f7f6">

Then I tested the same command after enabling the internet connection and I got this:

<img width="374" alt="Screenshot 2024-09-11 at 23 58 43" src="https://github.com/user-attachments/assets/b5dd36b3-125d-45ea-b526-836ffcc4005e">

## c)  Local only. Portscan your own computer using "localhost" address. It's illegal to portscan computers you don't own. Disconnect computer from the Internet while testing.

For this task I installed the nmap. I used "sudo apt-get install nmap" command.


<img width="473" alt="Screenshot 2024-09-12 at 0 04 32" src="https://github.com/user-attachments/assets/16329873-16d6-4d12-912e-87e1ecc265ff">


This is the results i got:



<img width="533" alt="Screenshot 2024-09-12 at 0 05 39" src="https://github.com/user-attachments/assets/34db4c85-0d76-454f-9a7b-f89846792c1b">

After this I have been stuck and I couldn't figure out what's wrong. I tried to restart but I got the same results.


References:

https://www.youtube.com/watch?v=Nh7OrFVyDo0&t=153s
https://terokarvinen.com/information-security/#h3-hack-to-learn-hacking


