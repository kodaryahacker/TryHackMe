# TryHackMe: Brooklyn Nine Nine Room Writeup

---

1. **User flag**  
   **Ans:** `ee11cbb19052e40b07aac0ca060c23ee`
   
On performing nmap scan, we can see that anonymous login is allowed for ftp.

<img width="856" height="686" alt="image" src="https://github.com/user-attachments/assets/2795c430-7e52-478c-b0c8-ee70db06480f" />

Login using the username and password as ‘anonymous’.

Extract the file found using ‘get’ command.

<img width="1100" height="475" alt="image" src="https://github.com/user-attachments/assets/6a1fe0ee-3a38-41f6-9aab-31d0db572f3c" />

It seems, we can find the password of the user jake. Let’s use hydra.

<img width="1100" height="180" alt="image" src="https://github.com/user-attachments/assets/a97b6e20-eb5f-4f97-b148-1aeaca319d38" />

Now let’s use these credentials to login to the ssh which is found to be open through the nmap scan.

<img width="491" height="717" alt="image" src="https://github.com/user-attachments/assets/1e80964a-3bef-4700-ab28-32c3a6c05dd1" />



3. **Root flag**  
   **Ans:** `63a9f0ea7bb98050796b649e85481845`

<img width="1100" height="175" alt="image" src="https://github.com/user-attachments/assets/6bc3235b-43aa-47a3-b9ad-36d0c45635f2" />

Use Gtfobins.

<img width="1100" height="501" alt="image" src="https://github.com/user-attachments/assets/f6c4198d-ac03-4eff-a130-1787d05617d8" />

<img width="1032" height="272" alt="image" src="https://github.com/user-attachments/assets/cada58c9-dbb5-409b-a4be-60def493086a" />

Enter the above command in the terminal.

<img width="873" height="731" alt="image" src="https://github.com/user-attachments/assets/42a0c238-61b6-4a74-b1f2-6dc600f31642" />

<img width="829" height="607" alt="image" src="https://github.com/user-attachments/assets/09b06d08-aae8-49e0-bbe9-136280140c4c" />

The other way to find the user and root flags.

This is the webpage given to us.

<img width="1100" height="478" alt="image" src="https://github.com/user-attachments/assets/2422a257-03c0-4cca-9d0c-f6f74fb1c6b5" />

On inspecting it, we can find a clue to use steganography. Download the above image.

<img width="1081" height="568" alt="image" src="https://github.com/user-attachments/assets/4c7991d2-bb89-480a-ae96-3df62e79ad78" />

<img width="850" height="460" alt="image" src="https://github.com/user-attachments/assets/362e8da5-23eb-4990-b15c-06390217a541" />

The password was found to be admin. On reading the file extracted, a password for the user holt was found. Use these credentials to login to ssh.

<img width="648" height="664" alt="image" src="https://github.com/user-attachments/assets/50922075-c682-4688-a27a-4ff17d4e7811" />

The user flag is found.

<img width="1100" height="112" alt="image" src="https://github.com/user-attachments/assets/693f93f8-5faf-413e-9a6f-8f35a06c5d3c" />

Use Gtfobins.

<img width="1100" height="548" alt="image" src="https://github.com/user-attachments/assets/8bab825c-f281-4ba4-89f6-85f440f85db5" />

<img width="1039" height="260" alt="image" src="https://github.com/user-attachments/assets/2ed8f9e6-617f-481e-a64f-144c0168488e" />

<img width="1100" height="732" alt="image" src="https://github.com/user-attachments/assets/bd585b41-107a-4c30-b148-66087ba4329b" />

<img width="563" height="305" alt="image" src="https://github.com/user-attachments/assets/2735dc4b-0702-4943-9029-907ca615e8f0" />

Or

<img width="543" height="163" alt="image" src="https://github.com/user-attachments/assets/ed525885-071a-4cc1-86f5-fb4dbae56132" />

The root flag is also successfully found!!

