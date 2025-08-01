# TryHackMe: Bounty Hacker Room Writeup

---

**1. Deploy the machine.**

Ans. `No answer needed`

---


**2. Find open ports on the machine**

<img width="991" height="722" alt="image" src="https://github.com/user-attachments/assets/681b80a0-ba0b-4770-8836-d2e2479a4707" />

---


**3. Who wrote the task list?**

Ans. `lin`

Login to the ftp as anonymous and we can find 2 files, download them using ‘get’ command.

<img width="1093" height="727" alt="image" src="https://github.com/user-attachments/assets/721b51a0-e3dc-4b94-a8f4-e200518c3f13" />

On reading the task.txt, we can find that the file is written by ‘lin’.

<img width="594" height="154" alt="image" src="https://github.com/user-attachments/assets/06c82e92-7037-448c-b5a4-4150ed37f09f" />

---


**4. What service can you bruteforce with the text file found?**

Ans. `SSH`

From the nmap scan performed, the SSH port is found to be open, so we can probably bruteforce to find the password.

<img width="594" height="577" alt="image" src="https://github.com/user-attachments/assets/a23610de-1908-466b-96eb-08412dd39e7f" />

---


**5. What is the users password?**

Ans. `RedDr4gonSynd1cat3`

<img width="1100" height="166" alt="image" src="https://github.com/user-attachments/assets/665b62dd-8c94-47ec-b8ee-9e417308618c" />

---


**6. user.txt**

Ans. `THM{CR1M3_SyNd1C4T3}`

On logging into SSH using the credentials obtained, we can find the user flag.

<img width="835" height="548" alt="image" src="https://github.com/user-attachments/assets/97fc3d98-9bd2-4125-8815-8f7a551ea5cd" />

---


**7. root.txt**

Ans. `THM{80UN7Y_h4cK3r}`

Use sudo -l command. We can find that the tar directory has root privileges.

<img width="972" height="657" alt="image" src="https://github.com/user-attachments/assets/4a8afaf9-31ce-4175-b7fc-de11ac166a7a" />

Now, use Gtfobins.

<img width="1100" height="497" alt="image" src="https://github.com/user-attachments/assets/65acbd88-b32e-4a35-bcba-b55f586f2623" />

<img width="1027" height="232" alt="image" src="https://github.com/user-attachments/assets/aa968c90-f65a-415c-b673-cf7d5fe51973" />

Run the above command in the terminal.

<img width="1012" height="701" alt="image" src="https://github.com/user-attachments/assets/35b9d6e7-e568-4bf1-a8ab-3e635df28727" />

The root flag is also successfully obtained.

