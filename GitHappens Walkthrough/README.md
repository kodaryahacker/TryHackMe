# TryHackMe GitHappens Room Writeup

## Boss wanted me to create a prototype, so here it is! We even used something called “version control” that made deploying this really easy!

<img width="383" height="383" alt="image" src="https://github.com/user-attachments/assets/cee9ac68-7018-4eaf-887a-824c351c1708" />

I started by downloading the git directory into my local kali machine using the command below.


```
wget -r --no-parent http://10.10.44.0/.git
```

The command recursively downloads the entire `.git` directory and its contents from the specified URL, avoiding traversal to parent directories.

<img width="828" height="387" alt="image" src="https://github.com/user-attachments/assets/389595d7-db71-428a-94a8-84050cb14ac7" />

```
cd <ip>
```

Navigate to the directory that was downloaded where you can find the `.git` directory.

<img width="828" height="632" alt="image" src="https://github.com/user-attachments/assets/4311f267-73cb-4e07-bf0c-45a4da08e4c0" />

```
git log
```

The `git log` command displays the commit history of the repository, showing details like commit hashes, authors, dates, and messages.

<img width="828" height="572" alt="image" src="https://github.com/user-attachments/assets/e16f781c-c6c1-4867-bbc5-47881e117b49" />

<img width="753" height="735" alt="image" src="https://github.com/user-attachments/assets/5a759736-471f-4c4c-82f3-d10b5ea55b10" />

<img width="629" height="336" alt="image" src="https://github.com/user-attachments/assets/366f8c97-15aa-457c-8bff-70634ef1d474" />

There was a commit made which says `Made the login page, boss!` . I felt it might hold the clue to our password.

```
git show <commit-hash>
```

The `git show` command displays detailed information about a specific commit, including changes made, the commit message, and metadata like the author and timestamp.

<img width="760" height="426" alt="image" src="https://github.com/user-attachments/assets/a3631940-6d9d-44ea-8d25-590f6400261a" />

<img width="828" height="595" alt="image" src="https://github.com/user-attachments/assets/b9409577-cb95-4ff8-91a7-2b0244bea86c" />

Successfully, found the password. It’s a very good beginner friendly room, try it out!! Happy Hacking!!!🧑‍💻
