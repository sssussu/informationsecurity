
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


