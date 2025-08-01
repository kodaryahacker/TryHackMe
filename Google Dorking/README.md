# TryHackMe: Google Dorking Room Writeup

Here is the writeup for the **Google Dorking** room of TryHackMe…

---

## Task 1  
**“Roger dogder”**  
**Ans:** No answer needed

---

## Task 2

1. **Name the key term of what a “Crawler” is used to do**  
   **Ans:** `index`

2. **What is the name of the technique that “Search Engines” use to retrieve this information about websites?**  
   **Ans:** `Crawling`

3. **What is an example of the type of contents that could be gathered from a website?**  
   **Ans:** `Keywords`

---

## Task 3

**Use the same SEO checkup tool and other online alternatives to see how their results compare for:**  
- `https://tryhackme.com`  
- `http://googledorking.cmnatic.co.uk`  

**Ans:** No answer needed

---

## Task 4

1. **Where would “robots.txt” be located on the domain “ablog.com”?**  
   **Ans:** `ablog.com/robots.txt`

2. **If a website was to have a sitemap, where would that be located?**  
   **Ans:** `/sitemap.xml`

3. **How would we only allow “Bingbot” to index the website?**  
   **Ans:**
   ```
   User-agent: Bingbot
   ```

4. **How would we prevent a “Crawler” from indexing the directory “/dont-index-me/”?**  
   **Ans:**
   ```
   Disallow: /dont-index-me/
   ```

5. **What is the extension of a Unix/Linux system configuration file that we might want to hide from “Crawlers”?**  
   **Ans:** `.conf`

---

## Task 5

1. **What is the typical file structure of a “Sitemap”?**  
   **Ans:** `XML`

2. **What real life example can “Sitemaps” be compared to?**  
   **Ans:** `Map`

3. **Name the keyword for the path taken for content on a website**  
   **Ans:** `Route`

---

## Task 6

1. **What would be the format used to query the site bbc.co.uk about flood defences?**  
   **Ans:** `site: bbc.co.uk flood defences`

2. **What term would you use to search by file type?**  
   **Ans:** `filetype:`

3. **What term can we use to look for login pages?**  
   **Ans:** `intitle: login`

---
